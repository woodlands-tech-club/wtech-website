<script>
	import { onMount } from "svelte";



    let canvas;
    let rect_width = 80;
    let rect_height = 80;
    let ctx;
    let rect_stack = [];
    let deactivated_color = "rgba(20, 20, 20, 1)";
    let activate_color = "rgb(43, 29, 117)";
    let last_rect = {x: 0, y: 0};

    const draw_rect = (ctx, x, y, width, height, color) => {
        ctx.strokeStyle = color;
        ctx.strokeRect(x, y, width, height);
    }

    const fill_rectangle_pattern = (ctx, width, height, color) => {
        for (let y = 0; y <= window.innerHeight; y+=rect_height){
            for (let x = 0; x <= window.innerWidth; x+=rect_width){
                draw_rect(ctx, x, y, width, height, color);
            }
        }
    }

    const clamp = (n, increment) => {
        return n - (n % increment);
    }

    const activateRect = (e) => {
        let mouse = {x: 0, y: 0};
        mouse.x = e.clientX;
        mouse.y = e.clientY;
        let x = clamp(mouse.x, rect_width);
        let y = clamp(mouse.y, rect_height);
        if (last_rect.x == x && last_rect.y == y){
            return;
        }

        draw_rect(ctx, x, y, rect_width, rect_height, activate_color);

        rect_stack.unshift({x: x, y: y, width: rect_width, height: rect_height, color: activate_color})
        last_rect = {x: x, y: y};
    }

    const clearRectStack = () => {
        for (let i = 0; i < 10; i++){
            if (!rect_stack.length){
                return;
            }
            let rect = rect_stack.pop();
            draw_rect(ctx, rect.x, rect.y, rect.width, rect.height, deactivated_color);

        }
        rect_stack.forEach((n) => {
            draw_rect(ctx, n.x, n.y, n.width, n.height, n.color);
        })
    }

    setInterval(clearRectStack, 700)

    onMount(()=>{
        ctx = canvas.getContext("2d");
        ctx.canvas.width  = window.innerWidth;
        ctx.canvas.height = window.innerHeight;
        ctx.globalAlpha = 1;
        ctx.fillStyle = "black";
        ctx.lineWidth = 2;

        ctx.fillRect(0, 0, window.innerWidth, window.innerHeight); 
        fill_rectangle_pattern(ctx, rect_width, rect_height, deactivated_color)
        

    })
</script>

<canvas bind:this={canvas} class="fixed z-[-100000]"></canvas>
<div on:mousemove={activateRect} id="event_catcher" class="z-[10000] fixed w-[100%] h-[100%] pointer-events-none"></div>
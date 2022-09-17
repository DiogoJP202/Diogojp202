# Olá Mundo!! Meu nome é Diogo Antonny, estudante de programação e de desenvolvimento de sites!!

<p>👋 OII!! Sou Diogojp</p> 
<p>👀 Ainda pretendo estudar muitas coisas, uma delas é Back-end.</p> 
<p>🌱 Atualmente estou estudando Front-end.</p> 
<p>&#x1F3AE Gosto muito de jogos eletrônicos.</p> 

 <div>
    <a href="https://github.com/DiogoJP202">
    <img height="180em" src="https://github-readme-stats.vercel.app/api?username=DiogoJP202&show_icons=true&theme=dark&include_all_commits=true&count_private=true"/>
    <img height="180em" src="https://github-readme-stats.vercel.app/api/top-langs/?username=DiogoJP202&layout=compact&langs_count=7&theme=dark"/>
 </div> 
  
 <div>
    <br>
    <img align="center" alt="Diogo-HTML" height="50" width="60" src="https://cdn.jsdelivr.net/gh/devicons/devicon/icons/html5/html5-original.svg">
    <img align="center" alt="Diogo-CSS" height="50" width="60" src="https://cdn.jsdelivr.net/gh/devicons/devicon/icons/css3/css3-original.svg">
    <img align="center" alt="Diogo-JS" height="50" width="60" src="https://cdn.jsdelivr.net/gh/devicons/devicon/icons/javascript/javascript-original.svg">
    <img align="center" alt="Diogo-C++" height="50" width="60" src="https://cdn.jsdelivr.net/gh/devicons/devicon/icons/cplusplus/cplusplus-original.svg">
    <img align="right" alt="Diogo-pic" height="150" style="border-radius:50px;" src="https://media.discordapp.net/attachments/553585426464768021/957332657216315452/94097_1xpZ4mSp.png?width=492&height=492">
  </div>
  <br>
  <div>
    <a href="https://www.youtube.com/channel/UCmHyxuA34292pxKtAguPA-Q" target="_blank" rel="external"><img src="https://img.shields.io/badge/YouTube-FF0000?style=for-the-badge&logo=youtube&logoColor=white" target="_blank"></a>
    <a href="https://www.instagram.com/ton.nyx3/" target="_blank" rel="external"><img src="https://img.shields.io/badge/-Instagram-%23E4405F?style=for-the-badge&logo=instagram&logoColor=white" target="_blank"></a>
    <a href="https://www.twitch.tv/dioogojp" target="_blank" rel="external"><img src="https://img.shields.io/badge/Twitch-9146FF?style=for-the-badge&logo=twitch&logoColor=white" target="_blank"></a>
    <a href="https://discord.gg/PXg266g8" target="_blank" rel="external"><img src="https://img.shields.io/badge/Discord-7289DA?style=for-the-badge&logo=discord&logoColor=white" target="_blank"></a> 
    <a href = "Diogojp202@gmai.com"><img src="https://img.shields.io/badge/-Gmail-%23333?style=for-the-badge&logo=gmail&logoColor=white" target="_blank" rel="external"></a>
    <a href="https://www.linkedin.com/in/diogo-antonny-8a65281b8/" target="_blank" rel="external"><img src="https://img.shields.io/badge/-LinkedIn-%230077B5?style=for-the-badge&logo=linkedin&logoColor=white" target="_blank"></a> 
    <img alt="Vagabond" height="auto" style=" width:100%; margin:auto; display:block;" src="https://media.discordapp.net/attachments/553585426464768021/1020457661910745138/o9z0g4vezev81.jpeg" id="Vagabond">
    
  ![Snake animation](https://github.com/rafaballerini/rafaballerini/blob/output/github-contribution-grid-snake.svg)

   
    <canvas id="stage" width="600" height="600"></canvas>
    <script type="text/javascript">
        
        window.onload = function(){
 
            var stage = document.getElementById('stage');
            var ctx = stage.getContext("2d");
            document.addEventListener("keydown", keyPush);
            setInterval(game, 80);
 
            const vel = 1;
 
            var vx = vy = 0;
            var px =10;
            var py = 15;
            var tp = 30;
            var qp = 20;
            var ax=ay=15;
 
            var trail = [];
            tail = 5;
 
            function game(){
                px += vx;
                py += vy;
                if (px <0) {
                    px = qp-1;
                }
                if (px > qp-1) {
                    px = 0;
                }
                if (py < 0) {
                    py = qp-1;
                }
                if (py > qp-1) {
                    py = 0;
                }
 
                ctx.fillStyle = "black";
                ctx.fillRect(0,0, stage.width, stage.height);
 
                ctx.fillStyle = "red";
                ctx.fillRect(ax*tp, ay*tp, tp,tp);
 
                ctx.fillStyle = "gray";
                for (var i = 0; i < trail.length; i++) {
                    ctx.fillRect(trail[i].x*tp, trail[i].y*tp, tp-1,tp-1);
                    if (trail[i].x == px && trail[i].y == py)
                    {
                        vx = vy=0;
                        tail =5;
                    }
                }
 
                trail.push({x:px,y:py })
                while (trail.length > tail) {
                    trail.shift();
                }
 
                if (ax==px && ay==py){
                    tail++;
                    ax = Math.floor(Math.random()*qp);
                    ay = Math.floor(Math.random()*qp);
                }
 
            }
 
            function keyPush(event){
 
                switch (event.keyCode) {
                    case 37: // Left
                        vx = -vel;
                        vy = 0;
                        break;
                    case 38: // up
                        vx = 0;
                        vy = -vel;
                        break;
                    case 39: // right
                        vx = vel;
                        vy = 0;
                        break;
                    case 40: // down
                        vx = 0;
                        vy = vel;
                        break;          
                    default:
                        
                        break;
                }
 
 
            }
 
        }
 
    </script>
    
  </div>
    

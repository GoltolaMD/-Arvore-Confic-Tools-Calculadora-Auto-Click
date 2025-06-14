# -Arvore-Confic-Tools-Calculadora-Auto-Click

# ✅ Calculadora de Cliques + Auto Click
Tudo em uma interface flutuante, fácil, rápida e prática!

# 🔥 Código Completo (Copiar tudo)

````javascript:(()=>{if(document.getElementById('arvoreConficUI'))return;let mouseX=0,mouseY=0;document.addEventListener("mousemove",e=>{mouseX=e.clientX;mouseY=e.clientY;});const style=document.createElement("style");style.innerHTML=`#arvoreConficUI{position:fixed;top:20px;right:20px;background:rgba(20,30,40,0.9);color:#ccf;padding:15px;border-radius:16px;box-shadow:0 0 15px rgba(0,255,180,0.6);font-family:Sans-Serif;backdrop-filter:blur(6px);max-width:320px;z-index:999999;}#arvoreConficUI input{width:60px;margin:4px;}#arvoreConficUI button{margin-top:6px;background:#00d8a4;color:#003e3e;border:none;padding:5px 10px;border-radius:8px;cursor:pointer;}#arvoreConficUI button:hover{opacity:0.8;}#arvoreConficUI .closeBtn{background:#f44;color:#fff;}#arvoreConficUI .section{margin-bottom:12px;padding-bottom:8px;border-bottom:1px solid #555;}#arvoreConficUI .section:last-child{border:none;}#arvoreConficUI label{color:#aef;}#arvoreConficUI .result{color:#dff;margin-top:6px;}@keyframes clickPulse{0%{transform:translate(-50%,-50%)scale(1);opacity:1;}100%{transform:translate(-50%,-50%)scale(2);opacity:0;}}.click-visual{position:fixed;width:20px;height:20px;background:rgba(0,255,0,0.5);border-radius:50%;pointer-events:none;transform:translate(-50%,-50%);animation:clickPulse 0.3s ease-out;z-index:999999;}`;document.head.appendChild(style);const UI=document.createElement("div");UI.id="arvoreConficUI";UI.innerHTML=`<div style="display:flex;justify-content:space-between;align-items:center;"><b style="color:#90fcd2;">🖱️🎯 Arvore Confic Tools</b><button class="closeBtn">X</button></div><div class="section"><div style="font-weight:bold;margin-bottom:6px;">🧠 Calculadora 15min</div><label>Total de Cliques:</label><input id="totalClicksInput" type="number" min="1"><button id="calcClickBtn">Calcular</button><div id="clickResult" class="result"></div></div><div class="section"><div style="font-weight:bold;margin-bottom:6px;">🎯 Auto Click</div><label>Cliques por segundo:</label><input type="number" id="cpsInput" value="5" min="1" max="100"><div style="font-size:12px;margin-top:6px;"><b>F6</b> = Iniciar • <b>F7</b> = Parar</div><button id="toggleBtn">Iniciar</button></div>`;document.body.appendChild(UI);UI.querySelector(".closeBtn").onclick=()=>{UI.remove();style.remove();clearInterval(intervalId);};UI.querySelector("#calcClickBtn").onclick=()=>{const total=parseInt(document.getElementById('totalClicksInput').value);const result=document.getElementById('clickResult');if(isNaN(total)||total<=0){result.innerHTML=`<span style="color:#ff8080;">❌ Número inválido</span>`;return;}const totalSegundos=15*60;const cps=total/totalSegundos;const intervalo=totalSegundos/total;result.innerHTML=`🕒 Tempo Total: <b>15 minutos</b><br>👆 Total de Cliques: <b>${total}</b><br><br>➡️ <b>${cps.toFixed(4)}</b> cliques por segundo<br>⏱️ <b>${intervalo.toFixed(2)}</b> segundos por clique`;};let clicking=false;let intervalId;function showClickEffect(x,y){const dot=document.createElement("div");dot.className="click-visual";dot.style.left=x+"px";dot.style.top=y+"px";document.body.appendChild(dot);setTimeout(()=>dot.remove(),300);}function startClicking(){if(clicking)return;const cps=parseFloat(document.getElementById("cpsInput").value);if(isNaN(cps)||cps<=0){alert("CPS inválido");return;}clicking=true;UI.querySelector("#toggleBtn").textContent="Parar";intervalId=setInterval(()=>{const el=document.elementFromPoint(mouseX,mouseY);if(el){const evt=new MouseEvent("click",{bubbles:true,cancelable:true,view:window});el.dispatchEvent(evt);showClickEffect(mouseX,mouseY);}},1000/cps);}function stopClicking(){if(!clicking)return;clicking=false;clearInterval(intervalId);UI.querySelector("#toggleBtn").textContent="Iniciar";}function toggleClicking(){clicking?stopClicking():startClicking();}document.getElementById("toggleBtn").onclick=toggleClicking;document.addEventListener("keydown",e=>{if(e.code==="F6")startClicking();if(e.code==="F7")stopClicking();});
})();

# 🚀 Como Usar
Crie um favorito no navegador.

No campo de URL, cole todo o código acima (começando com javascript:).

Clique no favorito em qualquer site.

A interface vai aparecer no canto direito superior.

# ✅ Use a Calculadora de Cliques para saber:

Quantos cliques por segundo.

Qual intervalo entre cada clique.

# ✅ Use o Auto Click:

Configure os cliques por segundo.

Clique em Iniciar ou pressione F6.

Para parar, clique em Parar ou pressione F7.

# ⚙️ Recursos
🧠 Calculadora de Cliques:
Calcula a quantidade de cliques por segundo e o intervalo entre cliques para 15 minutos.

🎯 Auto Click:
Realiza cliques automáticos na posição atual do mouse com efeito visual de clique.

# -Arvore-Confic-Tools-Calculadora-Auto-Click

# ✅ Calculadora de Cliques + Auto Click
Tudo em uma interface flutuante, fácil, rápida e prática!

# 🔥 Código Completo (Copiar tudo)

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

````javascript
javascript:(function()%7Bjavascript%3A(()%3D%3E%7Bif(document.getElementById('arvoreConficUI'))return%3Blet%20mouseX%3D0%2CmouseY%3D0%3Bdocument.addEventListener(%22mousemove%22%2Ce%3D%3E%7BmouseX%3De.clientX%3BmouseY%3De.clientY%3B%7D)%3Bconst%20style%3Ddocument.createElement(%22style%22)%3Bstyle.innerHTML%3D%60%23arvoreConficUI%7Bposition%3Afixed%3Btop%3A20px%3Bright%3A20px%3Bbackground%3Argba(20%2C30%2C40%2C0.9)%3Bcolor%3A%23ccf%3Bpadding%3A15px%3Bborder-radius%3A16px%3Bbox-shadow%3A0%200%2015px%20rgba(0%2C255%2C180%2C0.6)%3Bfont-family%3ASans-Serif%3Bbackdrop-filter%3Ablur(6px)%3Bmax-width%3A320px%3Bz-index%3A999999%3B%7D%23arvoreConficUI%20input%7Bwidth%3A60px%3Bmargin%3A4px%3B%7D%23arvoreConficUI%20button%7Bmargin-top%3A6px%3Bbackground%3A%2300d8a4%3Bcolor%3A%23003e3e%3Bborder%3Anone%3Bpadding%3A5px%2010px%3Bborder-radius%3A8px%3Bcursor%3Apointer%3B%7D%23arvoreConficUI%20button%3Ahover%7Bopacity%3A0.8%3B%7D%23arvoreConficUI%20.closeBtn%7Bbackground%3A%23f44%3Bcolor%3A%23fff%3B%7D%23arvoreConficUI%20.section%7Bmargin-bottom%3A12px%3Bpadding-bottom%3A8px%3Bborder-bottom%3A1px%20solid%20%23555%3B%7D%23arvoreConficUI%20.section%3Alast-child%7Bborder%3Anone%3B%7D%23arvoreConficUI%20label%7Bcolor%3A%23aef%3B%7D%23arvoreConficUI%20.result%7Bcolor%3A%23dff%3Bmargin-top%3A6px%3B%7D%40keyframes%20clickPulse%7B0%25%7Btransform%3Atranslate(-50%25%2C-50%25)scale(1)%3Bopacity%3A1%3B%7D100%25%7Btransform%3Atranslate(-50%25%2C-50%25)scale(2)%3Bopacity%3A0%3B%7D%7D.click-visual%7Bposition%3Afixed%3Bwidth%3A20px%3Bheight%3A20px%3Bbackground%3Argba(0%2C255%2C0%2C0.5)%3Bborder-radius%3A50%25%3Bpointer-events%3Anone%3Btransform%3Atranslate(-50%25%2C-50%25)%3Banimation%3AclickPulse%200.3s%20ease-out%3Bz-index%3A999999%3B%7D%60%3Bdocument.head.appendChild(style)%3Bconst%20UI%3Ddocument.createElement(%22div%22)%3BUI.id%3D%22arvoreConficUI%22%3BUI.innerHTML%3D%60%3Cdiv%20style%3D%22display%3Aflex%3Bjustify-content%3Aspace-between%3Balign-items%3Acenter%3B%22%3E%3Cb%20style%3D%22color%3A%2390fcd2%3B%22%3E%F0%9F%96%B1%EF%B8%8F%F0%9F%8E%AF%20Arvore%20Confic%20Tools%3C%2Fb%3E%3Cbutton%20class%3D%22closeBtn%22%3EX%3C%2Fbutton%3E%3C%2Fdiv%3E%3Cdiv%20class%3D%22section%22%3E%3Cdiv%20style%3D%22font-weight%3Abold%3Bmargin-bottom%3A6px%3B%22%3E%F0%9F%A7%A0%20Calculadora%2015min%3C%2Fdiv%3E%3Clabel%3ETotal%20de%20Cliques%3A%3C%2Flabel%3E%3Cinput%20id%3D%22totalClicksInput%22%20type%3D%22number%22%20min%3D%221%22%3E%3Cbutton%20id%3D%22calcClickBtn%22%3ECalcular%3C%2Fbutton%3E%3Cdiv%20id%3D%22clickResult%22%20class%3D%22result%22%3E%3C%2Fdiv%3E%3C%2Fdiv%3E%3Cdiv%20class%3D%22section%22%3E%3Cdiv%20style%3D%22font-weight%3Abold%3Bmargin-bottom%3A6px%3B%22%3E%F0%9F%8E%AF%20Auto%20Click%3C%2Fdiv%3E%3Clabel%3ECliques%20por%20segundo%3A%3C%2Flabel%3E%3Cinput%20type%3D%22number%22%20id%3D%22cpsInput%22%20value%3D%225%22%20min%3D%221%22%20max%3D%22100%22%3E%3Cdiv%20style%3D%22font-size%3A12px%3Bmargin-top%3A6px%3B%22%3E%3Cb%3EF6%3C%2Fb%3E%20%3D%20Iniciar%20%E2%80%A2%20%3Cb%3EF7%3C%2Fb%3E%20%3D%20Parar%3C%2Fdiv%3E%3Cbutton%20id%3D%22toggleBtn%22%3EIniciar%3C%2Fbutton%3E%3C%2Fdiv%3E%60%3Bdocument.body.appendChild(UI)%3BUI.querySelector(%22.closeBtn%22).onclick%3D()%3D%3E%7BUI.remove()%3Bstyle.remove()%3BclearInterval(intervalId)%3B%7D%3BUI.querySelector(%22%23calcClickBtn%22).onclick%3D()%3D%3E%7Bconst%20total%3DparseInt(document.getElementById('totalClicksInput').value)%3Bconst%20result%3Ddocument.getElementById('clickResult')%3Bif(isNaN(total)%7C%7Ctotal%3C%3D0)%7Bresult.innerHTML%3D%60%3Cspan%20style%3D%22color%3A%23ff8080%3B%22%3E%E2%9D%8C%20N%C3%BAmero%20inv%C3%A1lido%3C%2Fspan%3E%60%3Breturn%3B%7Dconst%20totalSegundos%3D15*60%3Bconst%20cps%3Dtotal%2FtotalSegundos%3Bconst%20intervalo%3DtotalSegundos%2Ftotal%3Bresult.innerHTML%3D%60%F0%9F%95%92%20Tempo%20Total%3A%20%3Cb%3E15%20minutos%3C%2Fb%3E%3Cbr%3E%F0%9F%91%86%20Total%20de%20Cliques%3A%20%3Cb%3E%24%7Btotal%7D%3C%2Fb%3E%3Cbr%3E%3Cbr%3E%E2%9E%A1%EF%B8%8F%20%3Cb%3E%24%7Bcps.toFixed(4)%7D%3C%2Fb%3E%20cliques%20por%20segundo%3Cbr%3E%E2%8F%B1%EF%B8%8F%20%3Cb%3E%24%7Bintervalo.toFixed(2)%7D%3C%2Fb%3E%20segundos%20por%20clique%60%3B%7D%3Blet%20clicking%3Dfalse%3Blet%20intervalId%3Bfunction%20showClickEffect(x%2Cy)%7Bconst%20dot%3Ddocument.createElement(%22div%22)%3Bdot.className%3D%22click-visual%22%3Bdot.style.left%3Dx%2B%22px%22%3Bdot.style.top%3Dy%2B%22px%22%3Bdocument.body.appendChild(dot)%3BsetTimeout(()%3D%3Edot.remove()%2C300)%3B%7Dfunction%20startClicking()%7Bif(clicking)return%3Bconst%20cps%3DparseFloat(document.getElementById(%22cpsInput%22).value)%3Bif(isNaN(cps)%7C%7Ccps%3C%3D0)%7Balert(%22CPS%20inv%C3%A1lido%22)%3Breturn%3B%7Dclicking%3Dtrue%3BUI.querySelector(%22%23toggleBtn%22).textContent%3D%22Parar%22%3BintervalId%3DsetInterval(()%3D%3E%7Bconst%20el%3Ddocument.elementFromPoint(mouseX%2CmouseY)%3Bif(el)%7Bconst%20evt%3Dnew%20MouseEvent(%22click%22%2C%7Bbubbles%3Atrue%2Ccancelable%3Atrue%2Cview%3Awindow%7D)%3Bel.dispatchEvent(evt)%3BshowClickEffect(mouseX%2CmouseY)%3B%7D%7D%2C1000%2Fcps)%3B%7Dfunction%20stopClicking()%7Bif(!clicking)return%3Bclicking%3Dfalse%3BclearInterval(intervalId)%3BUI.querySelector(%22%23toggleBtn%22).textContent%3D%22Iniciar%22%3B%7Dfunction%20toggleClicking()%7Bclicking%3FstopClicking()%3AstartClicking()%3B%7Ddocument.getElementById(%22toggleBtn%22).onclick%3DtoggleClicking%3Bdocument.addEventListener(%22keydown%22%2Ce%3D%3E%7Bif(e.code%3D%3D%3D%22F6%22)startClicking()%3Bif(e.code%3D%3D%3D%22F7%22)stopClicking()%3B%7D)%3B%7D)()%7D)()

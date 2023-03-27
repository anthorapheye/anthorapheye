<style>
    h1 {
        position: fixed;
        top: 50%;
        left: 0;
        width: 100vw;
        transform: translateX(-50%, -50%);
        text-align: center;
        color: #f00;
        font-family: consolas;
        user-select: none;
    }
</style>
<h1></h1>
<script>
    const titre = document.querySelector("h1");
    const texte = "👁 Welcome to my Github page 👁";
    const img = new Image();
    img.src = "./autorun.ico";
    let i = 0;
    const timerID = setInterval(() => {
        titre.innerHTML += texte[i];
        i++;
        if (i === texte.length) clearInterval(timerID);
    }, 100);
</script>

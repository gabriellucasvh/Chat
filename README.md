# Chat feito com WebSockets
Caso queira usar, modifique o servidor em `script.js`
e use `wss://` ao invés de `https://`

    const handleLogin = (event) => {
    event.preventDefault()

    user.id = crypto.randomUUID()
    user.name = loginInput.value
    user.color = getRandomColor()

    login.style.display = "none"
    chat.style.display = "flex"

    websocket = new WebSocket("wss://SeuServidor") //aqui
    websocket.onmessage = processMessage
    }


![](https://i.imgur.com/H2UA1Oy.png)
![](https://i.imgur.com/1V2v71R.png)
![](https://i.imgur.com/qlyMSUF.png)

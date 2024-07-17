# ex3-java
## home.html
```c
<!DOCTYPE html>
<html lang="en">
<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>Simplified Dribbble Clone</title>
    <link rel="stylesheet" href="style.css">
</head>
<body>
    <header>
        <div class="container">
            <div class="logo">Dribbble</div>
            <nav>
                <ul>
                    <li><a href="#">Shots</a></li>
                    <li><a href="#">Designers</a></li>
                    <li><a href="#">Teams</a></li>
                    <li><a href="#">Community</a></li>
                    <li><a href="#">Jobs</a></li>
                </ul>
            </nav>
            <div class="auth-buttons">
                <button class="signup">Sign up</button>
                <button class="signin">Sign in</button>
            </div>
        </div>
    </header>
    <main>
        <div class="search-bar">
            <input type="text" placeholder="">
            <button class="learn-more">Search</button>
        </div>
        <section class="shots">
            <div class="shot">
                <img src="1.png" alt="Shot 1">
                <div class="shot-info">
                    <div class="title">Website for Manufacuring</div>
                    <div class="likes">❤ 4,044</div>
                </div>
            </div>
            <div class="shot">
                <img src="2.png" alt="Shot 2">
                <div class="shot-info">
                    <div class="title">DKNG</div>
                    <div class="likes">❤ 2,404</div>
                </div>
            </div>
            <div class="shot">
                <img src="3.png" alt="Shot 3">
                <div class="shot-info">
                    <div class="title">DKNG</div>
                    <div class="likes">❤ 3,985</div>
                </div>
            </div>
            <div class="shot">
                <img src="4.png" alt="Shot 4">
                <div class="shot-info">
                    <div class="title">DKNG</div>
                    <div class="likes">❤ 2,602</div>
                </div>
            </div>
            <div class="shot">
                <img src="5.png" alt="Shot 5">
                <div class="shot-info">
                    <div class="title">Emir Ayouni</div>
                    <div class="likes">❤ 2,369</div>
                </div>
            </div>
            <div class="shot">
                <img src="6.png" alt="Shot 6">
                <div class="shot-info">
                    <div class="title">Rik Catlow</div>
                    <div class="likes">❤ 1,022</div>
                </div>
            </div>
            <div class="shot">
                <img src="7.png" alt="Shot 7">
                <div class="shot-info">
                    <div class="title">Web Redesign</div>
                    <div class="likes">❤ 5,414</div>
                </div>
            </div>
            <div class="shot">
                <img src="8.png" alt="Shot 8">
                <div class="shot-info">
                    <div class="title">Radio</div>
                    <div class="likes">❤ 4,237</div>
                </div>
            </div>
            <div class="shot">
                <img src="9.png" alt="Shot 9">
                <div class="shot-info">
                    <div class="title">Logo Concept</div>
                    <div class="likes">❤ 1,845</div>
                </div>
            </div>
            <div class="shot">
                <img src="10.png" alt="Shot 10">
                <div class="shot-info">
                    <div class="title">Passage</div>
                    <div class="likes">❤ 7,175</div>
                </div>
            </div>
            <div class="shot">
                <img src="11.png" alt="Shot 11">
                <div class="shot-info">
                    <div class="title">Rich & Creamy</div>
                    <div class="likes">❤ 4,272</div>
                </div>
            </div>
            <div class="shot">
                <img src="12.png" alt="Shot 12">
                <div class="shot-info">
                    <div class="title">Rocketech</div>
                    <div class="likes">❤ 4,527</div>
                </div>
            </div>
            <div class="shot">
                <img src="13.png" alt="Shot 13">
                <div class="shot-info">
                    <div class="title">Easy School</div>
                    <div class="likes">❤ 7,327</div>
                </div>
            </div>
            <div class="shot">
                <img src="14.png" alt="Shot 14">
                <div class="shot-info">
                    <div class="title">Gaia pitch deck</div>
                    <div class="likes">❤ 5,275</div>
                </div>
            </div>
            <div class="shot">
                <img src="15.png" alt="Shot 15">
                <div class="shot-info">
                    <div class="title">HR Dashboard</div>
                    <div class="likes">❤ 2,545</div>
                </div>
            </div>
                </div>
            </div>
        </section>
    </main>
</body>
</html>
```
## style.css:
```c
* {
    margin: 0;
    padding: 0;
    box-sizing: border-box;
}

body {
    font-family: 'Arial', sans-serif;
    background-color: #f5f5f5;
}

.container {
    display: flex;
    justify-content: space-between;
    align-items: center;
    padding: 20px;
    max-width: 1200px;
    margin: auto;
}

header {
    background-color: #333;
    color: white;
}

.logo {
    font-size: 24px;
    font-weight: bold;
}

nav ul {
    list-style: none;
    display: flex;
}

nav ul li {
    margin: 0 15px;
}

nav ul li a {
    color: white;
    text-decoration: none;
    position: relative;
}

nav ul li a::after {
    content: '';
    position: absolute;
    width: 0;
    height: 2px;
    background: #ea4c89;
    left: 0;
    bottom: -5px;
    transition: width 0.3s;
}

nav ul li a:hover::after {
    width: 100%;
}

.auth-buttons button {
    margin-left: 10px;
    padding: 10px 20px;
    border: none;
    cursor: pointer;
    transition: background 0.3s;
}

.auth-buttons .signup {
    background-color: #ea4c89;
    color: white;
}

.auth-buttons .signin {
    background-color: #fff;
    color: #322626;
}

.auth-buttons .signup:hover {
    background-color: #d43d72;
}

.auth-buttons .signin:hover {
    background-color: #f1f1f1;
}

main {
    max-width: 1200px;
    margin: auto;
    padding: 20px;
}

.search-bar {
    display: flex;
    justify-content: center;
    margin-bottom: 20px;
}

.search-bar input {
    width: 300px;
    padding: 10px;
    border: 1px solid #ccc;
    border-radius: 5px 0 0 5px;
    outline: none;
}

.search-bar button.learn-more {
    padding: 10px 20px;
    background-color: #ea4c89;
    border: none;
    color: white;
    border-radius: 0 5px 5px 0;
    cursor: pointer;
    transition: background 0.3s;
}

.search-bar button.learn-more:hover {
    background-color: #d43d72;
}

.shots {
    display: grid;
    grid-template-columns: repeat(auto-fill, minmax(200px, 1fr));
    gap: 20px;
}

.shot {
    background-color: white;
    padding: 10px;
    border-radius: 10px;
    box-shadow: 0 0 10px rgba(0, 0, 0, 0.1);
    transition: transform 0.3s, box-shadow 0.3s;
}

.shot:hover {
    transform: translateY(-5px);
    box-shadow: 0 0 20px rgba(0, 0, 0, 0.2);
}

.shot img {
    width: 100%;
    border-radius: 10px;
}

.shot-info {
    display: flex;
    justify-content: space-between;
    margin-top: 10px;
}

.title {
    font-size: 16px;
    font-weight: bold;
}

.likes {
    font-size: 14px;
    color: #ea4c89;
}
```
## OUTPUT:

![Screenshot 2024-07-17 113440](https://github.com/user-attachments/assets/004a47d4-3b8b-4f83-928d-302af4e54470)


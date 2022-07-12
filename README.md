- 👋 Hi, I’m @JoaoGabrielVS19
- 👀 I’m interested in ...
- 🌱 I’m currently learning ...
- 💞️ I’m looking to collaborate on ...
- 📫 How to reach me ...

<!---
JoaoGabrielVS19/JoaoGabrielVS19 is a ✨ special ✨ repository because its `README.md` (this file) appears on your GitHub profile.
You can click the Preview link to take a look at your changes.
--->

Skip to content
Search or jump to…
Pull requests
Issues
Marketplace
Explore
 
@JoaoGabrielVS19 
BlogCyberini
/
WebShareButton
Public
Code
Issues
1
Pull requests
Actions
Projects
Wiki
Security
Insights
WebShareButton/LinkedIn/linkedin-share-button.html
@HenriqueIni
HenriqueIni Update linkedin-share-button.html
Latest commit b375334 on 20 Jun 2018
 History
 1 contributor
56 lines (51 sloc)  4.75 KB

<!DOCTYPE html>
<!--
GitHub: HenriqueIni
https://www.blogcyberini.com/
-->
<html>
<head>
    <meta charset="utf-8">
    <title>Botão do LinkedIn</title>
    <!--
        A imagem do botão está em Base64 e foi obtida no IconFinder (https://www.iconfinder.com/icons/764981/linkedin_media_social_square_icon)
        Se preferir, coloque este CSS num arquivo externo.        
    -->
    <style>
        .linkedin-share-button{
            display: inline-block;            
            width: 40px;
            height: 40px;
            margin: 5px;
            background-size: 100% 100%; /* ou 'contain' */
            background-image: url("data:image/svg+xml;base64,PD94bWwgdmVyc2lvbj0iMS4wIiA/PjxzdmcgaGVpZ2h0PSI2MHB4IiB2ZXJzaW9uPSIxLjEiIHZpZXdCb3g9IjAgMCA2MCA2MCIgd2lkdGg9IjYwcHgiIHhtbG5zPSJodHRwOi8vd3d3LnczLm9yZy8yMDAwL3N2ZyIgeG1sbnM6c2tldGNoPSJodHRwOi8vd3d3LmJvaGVtaWFuY29kaW5nLmNvbS9za2V0Y2gvbnMiIHhtbG5zOnhsaW5rPSJodHRwOi8vd3d3LnczLm9yZy8xOTk5L3hsaW5rIj48dGl0bGUvPjxkZXNjLz48ZGVmcy8+PGcgZmlsbD0ibm9uZSIgZmlsbC1ydWxlPSJldmVub2RkIiBpZD0ic29pY2FsIiBzdHJva2U9Im5vbmUiIHN0cm9rZS13aWR0aD0iMSI+PGcgaWQ9InNvY2lhbCIgdHJhbnNmb3JtPSJ0cmFuc2xhdGUoLTc3My4wMDAwMDAsIC0xMzguMDAwMDAwKSI+PGcgaWQ9InNsaWNlcyIgdHJhbnNmb3JtPSJ0cmFuc2xhdGUoMTczLjAwMDAwMCwgMTM4LjAwMDAwMCkiLz48ZyBmaWxsPSIjMzQ2REE2IiBpZD0ic3F1YXJlLWZsYXQiIHRyYW5zZm9ybT0idHJhbnNsYXRlKDE3My4wMDAwMDAsIDEzOC4wMDAwMDApIj48cGF0aCBkPSJNNjAyLjk5NTkzNywwIEw2NTcuMDA0MDYzLDAgQzY1OC42NTg2NzMsMCA2NjAsMS4zMzczMDk3NCA2NjAsMi45OTU5Mzc0MyBMNjYwLDU3LjAwNDA2MjYgQzY2MCw1OC42NTg2NzMxIDY1OC42NjI2OSw2MCA2NTcuMDA0MDYzLDYwIEw2MDIuOTk1OTM3LDYwIEM2MDEuMzQxMzI3LDYwIDYwMCw1OC42NjI2OTAzIDYwMCw1Ny4wMDQwNjI2IEw2MDAsMi45OTU5Mzc0MyBDNjAwLDEuMzQxMzI2ODggNjAxLjMzNzMxLDAgNjAyLjk5NTkzNywwIFoiIGlkPSJzcXVhcmUtNyIvPjwvZz48ZyBmaWxsPSIjRkZGRkZGIiBpZD0iaWNvbiIgdHJhbnNmb3JtPSJ0cmFuc2xhdGUoMTgyLjAwMDAwMCwgMTUwLjAwMDAwMCkiPjxwYXRoIGQ9Ik02MTIuODgzMDc1LDMxLjgyMzE1MTIgTDYxMi44ODMwNzUsMTMuNTI0MzM4OSBMNjA3LjIyNzM3LDEzLjUyNDMzODkgTDYwNy4yMjczNywzMS44MjMxNTEyIEw2MTIuODgzMDc1LDMxLjgyMzE1MTIgWiBNNjEyLjg4MzA3NSw3LjAzODIxNDU1IEM2MTIuODQ5Mzg4LDUuNDAwNjU5OTYgNjExLjc1ODAxNiw0LjE1Mzg0NjE1IDYwOS45ODUwNTQsNC4xNTM4NDYxNSBDNjA4LjIxMTYzMiw0LjE1Mzg0NjE1IDYwNy4wNTI4ODUsNS40MDA2NTk5NiA2MDcuMDUyODg1LDcuMDM4MjE0NTUgQzYwNy4wNTI4ODUsOC42NDAyMDIzNCA2MDguMTc3OTQ0LDkuOTIzMDc2OTIgNjA5LjkxNzIxOSw5LjkyMzA3NjkyIEw2MDkuOTUwOTA2LDkuOTIzMDc2OTIgQzYxMS43NTgwMTYsOS45MjMwNzY5MiA2MTIuODgzMDc1LDguNjQwMjAyMzQgNjEyLjg4MzA3NSw3LjAzODIxNDU1IFogTTYyMi4xMTAwNDIsMzEuODIzMTUxNyBMNjIyLjExMDA0MiwyMS4zOTczNzI5IEM2MjIuMTEwMDQyLDIwLjgzOTQwMTQgNjIyLjE1MDM3LDIwLjI4MTQzIDYyMi4zMTQ0NDcsMTkuODgzNjY4MiBDNjIyLjc2MzAzNCwxOC43NjgyNzc4IDYyMy43ODM5NTYsMTcuNjEzNjYzNyA2MjUuNDk4MTk5LDE3LjYxMzY2MzcgQzYyNy43NDM4OTYsMTcuNjEzNjYzNyA2MjkuMTUyMjc4LDE4Ljg4ODE1ODcgNjI5LjE1MjI3OCwyMS4zOTczNzI3IEw2MjkuMTUyMjc4LDMxLjgyMzE1MTYgTDYzNC44NDYxNTQsMzEuODIzMTUxNyBMNjM0Ljg0NjE1NCwyMS4xMTgzODcyIEM2MzQuODQ2MTU0LDE1LjM4Mzk4NzggNjMxLjc4NTA0NSwxMi43MTU2NjkgNjI3LjcwMTkxLDEyLjcxNTY2OSBDNjI0LjM1NDA4MSwxMi43MTU2NjkgNjIyLjg4NDU3MiwxNC41ODczNTkzIDYyMi4wNjg2MDgsMTUuODYxMzAyIEw2MjIuMTA5NDg5LDEzLjQxMzkxMjMgTDYxNi40MjU0NjIsMTMuNDEzOTEyMyBDNjE2LjUwNzIyNCwxNS4xNjU3MjE1IDYxNi40MjU0NjIsMzEuODIzMTUxNiA2MTYuNDI1NDYyLDMxLjgyMzE1MTYgTDYyMi4xMTAwNDIsMzEuODIzMTUxNyBaIiBpZD0ibGlua2VkaW4iLz48L2c+PC9nPjwvZz48L3N2Zz4="); /*Base 64 Icon by Xinh Studio*/
            background-repeat: no-repeat;
            background-position: center;
        }        
    </style>
</head>

<body>
    <a href="" id="linkedin-share-btt" rel="nofollow" target="_blank" class="linkedin-share-button"></a>
    
    <!-- Você pode colocar este script num arquivo externo -->
    <script type="text/javascript">
        //Constrói a URL depois que o DOM estiver pronto
        document.addEventListener("DOMContentLoaded", function() {
            var url = encodeURIComponent(window.location.href); //url
            var titulo = encodeURIComponent(document.title); //título
            var linkedinLink = "https://www.linkedin.com/shareArticle?mini=true&url="+url+"&title="+titulo;
            
            //tenta obter o conteúdo da meta tag description
            var summary = document.querySelector("meta[name='description']");            
            summary = (!!summary)? summary.getAttribute("content") : null;
            
            //se a meta tag description estiver ausente...
            if(!summary){
                //...tenta obter o conteúdo da meta tag og:description
                summary = document.querySelector("meta[property='og:description']");
                summary = (!!summary)? summary.getAttribute("content") : null;
            }
            //altera o link do botão
            linkedinLink = (!!summary)? linkedinLink + "&summary=" + encodeURIComponent(summary) : linkedinLink;
            document.getElementById("linkedin-share-btt").href = linkedinLink;
        }, false);
    </script>
</body>

</html>
Footer
© 2022 GitHub, Inc.
Footer navigation
Terms
Privacy
Security
Status
Docs
Contact GitHub
Pricing
API
Training
Blog
About
You have no unread notifications

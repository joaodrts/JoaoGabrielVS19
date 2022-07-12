- 👋 Hi, I’m @JoaoGabrielVS19
- 👀 I’m interested in ...
- 🌱 I’m currently learning ...
- 💞️ I’m looking to collaborate on ...
- 📫 How to reach me ...

<!---
JoaoGabrielVS19/JoaoGabrielVS19 is a ✨ special ✨ repository because its `README.md` (this file) appears on your GitHub profile.
You can click the Preview link to take a look at your changes.
--->

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

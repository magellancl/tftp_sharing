<script>
    import action from '$lib/action.png';
    import { Email, HackerNews, Reddit, LinkedIn, Pinterest, Telegram, Tumblr, Vk, WhatsApp, Xing, Facebook, X, Line } from "svelte-share-buttons-component/src";

const url = 'https://team-planet.com/fr/fundraisings/coalition-companies';
const title = 'Opération TFTP';
const desc = `C’est LA plus grosse opération de l’année ! Si vous avez envie que les entreprises agissent pour le climat, à vous de jouer : https://team-planet.com/fr/fundraisings/coalition-companies 

Quand il s’agit de climat, vous avez probablement constaté qu’il n’est pas rare de lire que “les entreprises sont le problème”. 

En cette fin d’année, Team for the Planet (le plus grand mouvement d’action pour le climat en Europe) a lancé une opération hyper ambitieuse : réunir 10 000 sociétés, pour créer la plus grande coalition d’entreprises pour le climat au monde. Et tout ça, avant le 31 décembre ! 

Le message est simple : ensemble, aux côtés des citoyens, les entreprises ont le pouvoir de changer la donne ! Parce qu’elles font aussi partie de la solution. 

Team for the Planet l’a déjà prouvé avec plus de 115 000 actionnaires citoyens : quand chacun fait un petit pas, et que ces petits pas sont intelligemment synchronisés, l’impact peut être colossal. 

Il est temps que les entreprises s’unissent également à grande échelle pour le climat. 

Le temps de la demi-mesure et de la timidité est révolu. 
J’invite donc tous les chefs d’entreprises qui liront ce message à agir en rejoignant cette grande opération. 

J’invite également toutes les personnes qui me liront à faire circuler le message auprès de leurs employeurs et des chefs d’entreprise de leur réseau. 

Toute personne morale peut participer, il suffit pour cela de 2 minutes et 1000€.

Montrons que les entreprises sont capables d’être au rdv pour jouer un rôle important dans la transition écologique. Montrons au climat qu’on ne le laissera pas tomber ! 

Il n’est jamais trop tard pour faire mieux 💪

Pour participer et en savoir plus, tout se passe sur : https://team-planet.com/fr/fundraisings/coalition-companies 

#grandecoalition`;
const media = 'https://imgur.com/Q7Md6Jh';
</script>
<head>
    <style>
        * {
            margin: 0;
            padding: 0;
        }
        .imgbox {
            display: grid;
            height: 100%;
        }
        .center-fit {
            max-width: 100%;
            max-height: 100vh;
            margin: auto;
        }
    </style>
</head>
<body>
<div class="imgbox">
    <img class="center-fit" src='{action}' alt="Terre vu de l'espace. Texte : L'humain mène une guerre contre la nature. S'il gagne il est perdu. - Hubert Reeves">
<center>
<Email subject="{title}" body="{desc} {url}" />
<HackerNews class="share-button" {title} {url} />
<Reddit class="share-button" {title} {url} />
<LinkedIn class="share-button" {url} />
<Tumblr class="share-button" {title} {url} caption="{title}" />
<Pinterest class="share-button" {url} media={media} description={title} />
<Telegram class="share-button" text={title} {url} />
<Vk class="share-button" {title} {url} />
<WhatsApp class="share-button" text="{title} {url}" />
<Xing class="share-button" {title} {url} />
<Facebook class="share-button" quote="{title}" {url} />
<X class="share-button" text="{title}" {url} hashtags="grandecoalition" via="TFTP_France" related="other,users" />
<Line class="share-button" {url} />
</center>
</div>

</body>

<template>
    <div class="character">
        <div class="cardCharacter">
            <div class="face front">
                <img :src="character.image" :alt="character.name">
                <h6>{{character.name}}</h6>
            </div>
            <div class="face back">
                <div class="mt-4">
                    <h6>{{character.name}}</h6>
                </div>
                <small>Species: {{character.species}}</small>
                <small>Gender: {{character.gender}}</small>
                <small >Origin: {{character.origin.name}}</small>
                <small>Location: {{ character.location.name}}</small>
                <div class="link status">
                    <span class="m-2">{{character.status}}</span>
                    <span
                        :class="
                        character.status == 'Alive' ? 'fa-solid fa-heart-circle-check text-success' :
                        character.status == 'Dead' ? 'text-danger fa-solid fa-skull-crossbones' :
                        character.status == 'unknown' ? 'text-warning fa-solid fa-person-circle-question':
                        'default'
                        "
                    ><i class="fs-1"></i>                    
                    </span>
                </div>
            </div>
        </div>
    </div>
</template>

<script>
export default {
    props: ['character']
}
</script>

<style>
.character {
    margin: 20px;
}
.cardCharacter {
    position: relative;
    width: 250px;
    height: 300px;
}
.cardCharacter .face {
    position: absolute;
    width: 100%;
    height: 100%;
    backface-visibility: hidden;
    border-radius: 10px;
    overflow: hidden;
    transition: .5s;
}
.cardCharacter .front {
    transform: perspective(600px) rotateY(0deg);
    box-shadow: 0 5px 10px #000;
}

.cardCharacter .front img {
    position: absolute;
    width: 100%;
    height: 100%;
    object-fit: cover;
}

.cardCharacter .front h6 {
    position: absolute;
    top: 260px;
    width: 100%;
    height: 45px;
    line-height: 45px;
    color: white;
    background: rgba(0, 0, 0, .4);
    text-align: center;
}

.cardCharacter .back {
    transform: perspective(600px) rotateY(180deg);
    background: rgb(0, 0, 0);
    color: white;
    display: flex;
    flex-direction: column;
    justify-content: space-between;
    text-align: center;
    box-shadow: 0 5px 10px black;
}
.cardCharacter .back .link {
    border-top: solid 1px #f3f3f3;
    line-height: 100px;
}

.cardCharacter .back .link a {
    color: #f3f3f3;
}

.cardCharacter:hover .front {
    transform: perspective(600px) rotateY(180deg);
}

.cardCharacter:hover .back {
    transform: perspective(600px) rotateY(360deg);
}
</style>
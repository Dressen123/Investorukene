<div class="header">
    <div class="header_boks1">
        <p id = "headerskrift">Logo</p>
    </div>
    <div class="header_boks2">
        <p id = "headerskrift">Events</p>
    </div>
    <div class="header_boks3"></div>
    <div class="header_boks4"></div>
    <div class="header_boks5">
        <p id = "headerskrift">Logg inn</p>
    </div>
</div>
<div class="headerlinje"></div>

<slot/>

<style>
.header{
    width: 100%;
    height: 130px;
    background-color: #6e6a6f;
    display: flex;
    justify-content: center;
}

.header_boks1{
    height: 100%;
    width: 20%;
    display: flex;
    align-items: center;
    justify-content: center;
}
.header_boks2{
    height: 100%;
    width: 20%;
    display: flex;
    align-items: center;
    justify-content: center;
}
.header_boks3{
    height: 100%;
    width: 20%;

}
.header_boks4{
    height: 100%;
    width: 20%;
}
.header_boks5{
    height: 100%;
    width: 20%;
    display: flex;
    align-items: center;
    justify-content: center;
}

#headerskrift{
    color: #bcebcb;
    font-size: 2em;
}



.headerlinje{
    width: 100%;
    height: 10px;
    color: #bcebcb;
}

</style>
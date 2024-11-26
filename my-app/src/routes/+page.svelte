<div class="hjemside_kropp">
    <div class="hjemmsideboks1"></div>
    <div class="hjemmsideboks2">
        <p id="headerskrift">Velkommen til Eventra
            Oppdag spennende arrangementer og aktiviteter i nærheten av deg. 
            Planlegg, del og delta – alt samlet på ett sted. 
            Gjør hver dag til en opplevelse med Eventra!</p>
        <a href="/login-page">
            <button type="submit" class="button">Kom i gang</button>
        </a>
    </div>
    <div class="hjemmsideboks3"></div>
</div>
<slot/>

<style>
#headerskrift{
    color: #bcebcb;
    font-size: 2em;
}


.hjemside_kropp{
    width: 100%;
    height: 42em;
    background-color: #87d68d;
    display: flex;
    justify-content: space-between;
}

.button {
    background-color: #04AA6D;
    border: none;
    color: white;
    padding: 15px 32px;
    text-align: center;
    text-decoration: none;
    display: inline-block;
    font-size: 16px;
    margin: 4px 2px;
    cursor: pointer;
    border-radius: 15px;
}

.hjemmsideboks1{
    width: 30%;
    height: 100%;
}
.hjemmsideboks2{
    width: 40%;
    height: 100%;
    display: flex;
    flex-direction: column;
    justify-content: center;
    align-items: center;
}
.hjemmsideboks3{
    width: 30%;
    height: 100%;
}
</style>

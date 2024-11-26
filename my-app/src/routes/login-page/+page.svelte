<div class="kropp">
    <div class="brukernavn_boks">
        <label for="brukernavn" id="labelskrift">Brukernavn</label>
        <input type="text" id="brukernavn" placeholder="Skriv inn brukernavn" bind:value={brukernavn}>
    </div>
    
    <div class="passord_boks">
        <label for="passord" id="labelskrift">Passord</label>
        <input type="password" id="passord" placeholder="Skriv inn passord" bind:value={passord}>
    </div>
    
    <div class="logginn_knapp">
        <button class="button" on:click={logg_inn()}>Logg inn</button>
        <br>
        <p>{status}</p>
    </div>
</div>  

<script>

const loginDatabase = {
        kakemonster: "cookies",
        henrik: "appelsiner",
        smurfeis: "dyreparkis"
    };

    let brukernavn = '';
    let passord = '';
    let status = '';

    function logg_inn() {
        if (loginDatabase[brukernavn] === passord) {
            status = "LOGGET INN";
        } else {
            status = "IKKE LOGGET INN";
        }
    }
</script>

<style>
.kropp{
    width: 100%;
    height: 42em;
    background-color: #87d68d;
}

.brukernavn_boks,
.passord_boks {
    width: 100%;
    height: 150px; /* Slightly increased height for label + input space */
    display: flex;
    flex-direction: column; /* Stack label above the input */
    justify-content: center;
    align-items: center;
    gap: 10px; /* Space between label and input field */
}

#labelskrift {
    color: white;
    font-size: 1.5em; /* Adjust font size if needed */
    text-align: center; /* Optional: Center the label text */
}

#brukernavn,
#passord {
    height: 50px;
    width: 20%;
    font-size: 15pt;
}

.logginn_knapp {
    width: 100%;
    height: 50px;
    display: flex;
    justify-content: center;
    align-items: center;
}
.button {
    background-color: #6e6a6f;
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
</style>
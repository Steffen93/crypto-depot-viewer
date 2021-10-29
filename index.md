# Cryptocurrency Depot Viewer

Aktuell unterstützen wir nur den Binance Exchange

<input id="saveBinanceApiKey" type="text" placeholder="Binance Api Key"></input> <button>Speichern</button>

## Depot

| Coin | Symbol | Stückzahl | Aktueller Kurs / Wert | Einstandskurs / -wert | +/- in % |
|:-----|:-------|:----------|:----------------------|:----------------------|:---------|
| k.D. | k. D.  | k. D.     | k. D.                 | k. D.                 | k. D.    |

<style type="text/css">
  .page-header {
    background-image: none;
    background-color: orange;
  }
  h1 h2 h3 h4 h5 {
    color: inherit;
  }
</style>

<script>
  var save_button = document.getElementById('Save')
  save_button.onclick = saveData;

  function saveData(){
    var input = document.getElementById("saveBinanceApiKey");
    localStorage.setItem("binanceApiKey", input.value);
    var storedValue = localStorage.getItem("binanceApiKey");
    console.log("binanceApiKey: " + storedValue);
  }
</script>

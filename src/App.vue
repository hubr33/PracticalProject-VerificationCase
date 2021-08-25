<template>
  <div class="verificationCase">
    <div class="title">
      <h1>Weryfikacja spraw</h1>
    </div>
    <main>
      <div class="serviceAndRepair" v-if="serviceAndRepairVisible">
        <div class="oneServiceAndRepairReport">
          <div class="serviceFullname">
            <h2>Zgłaszający</h2>
            <p>Hubert</p>
            <p>Radziwonka</p>
          </div>
          <div class="techInfo">
            <h2>Dane zgłoszonego auta</h2>
            <div class="techWrapper">
              <div class="infoOne">
                <p>Marka: <span>BMW</span></p>
                <p>Model: <span>e90 2.0 163km (200km)</span></p>
                <p>Rok produkcji: <span>2005</span></p>
              </div>
              <div class="infoTwo">
                <p>Rodzja paliwa: <span>Diesel</span></p>
                <p>Stan licznika: <span>268000 KM</span></p>
                <p>Numer rejestracyjny: <span>WPN 1VY7</span></p>
              </div>
              <div class="vinInfo">
                <p>VIN</p>
                <span>YV1LFK2UCL1614743</span>
              </div>
              <div class="serviceDesc">
                Lorem ipsum dolor sit, amet consectetur adipisicing elit. Animi
                explicabo rem deleniti error ab reprehenderit excepturi iusto,
                minima iure, accusamus quibusdam in sunt harum odio obcaecati
                cumque nostrum. Illo, nesciunt!
              </div>
            </div>
          </div>
          <div class="serviceButtons">
            <button class="sendService">Wyślij</button>
            <button class="deleteService">Usuń</button>
          </div>
        </div>
      </div>

      <div class="fleetReport" v-if="newCarVisible">
        <div class="imgSection">
          <img
            src="https://lodz.premiumarena.pl/assets/samochodydemo/BMW-320-xDrive.jpg"
            alt=""
          />
        </div>
        <div class="fleetInfo">
          <h2>Informacje o aucie</h2>
          <div class="fleetWrapper">
            <div class="fleetOne">
              <p>Marka i model: <span>BMW e90 2.0D</span></p>
              <p>Moc: <span>200 KM</span></p>
              <p>Skrzynia: <span>Manualna</span></p>
              <p>Przyspieszenie: <span>6.5s</span></p>
            </div>
            <div class="fleetTwo">
              <p>Spalanie (trasa/miasto): <span>5/10l</span></p>
              <p>Liczba siedzeń: <span>5</span></p>
              <p>Rok produkcji: <span>2005</span></p>
              <p>Naped: <span>Tył</span></p>
            </div>
            <div class="fleetRentCosts">
              <div class="oneToFive">
                <p>1-5 dni</p>
                <p>500zł / dzień</p>
              </div>
              <div class="sixToThirteen">
                <p>6-13 dni</p>
                <p>400zł / dzień</p>
              </div>
              <div class="fourteenPlus">
                <p>14+ dni</p>
                <p>300zł / dzień</p>
              </div>
              <div class="fleetReposit">
                <p>Kaucja</p>
                <p>5000zł</p>
              </div>
            </div>
            <div class="fleetDescription">
              Lorem, ipsum dolor sit amet consectetur adipisicing elit. Unde
              quod ipsum quia adipisci perspiciatis iste. Esse non totam eos.
              Ducimus.
            </div>
          </div>
        </div>
        <div class="fleetButtons">
          <button class="addToFleet">Dodaj auto</button>
          <button class="doNotAddToFleet">Usuń zgłoszenie</button>
        </div>
      </div>
      <div class="issueReport" v-if="issueVisible">
        <div class="oneIssueReport">
          <div class="issueInfo">
            <p>Tytuł zgłoszenia: <span>Niedziałająca kasa</span></p>
            <p>Imię zgłaszającego: <span>Hubert</span></p>
            <p>Nazwisko zgłaszającego: <span>Radziwonka</span></p>
            <p>Data wystąpienia problemu: <span>23.08.2021</span></p>
          </div>
          <div class="issueDescription">
            Lorem, ipsum dolor sit amet consectetur adipisicing elit. Accusamus,
            ea alias! Eius eum laboriosam odio consequatur rerum nisi minima
            assumenda culpa quia doloremque, commodi iure. Dolorem voluptate at
            earum repellat saepe, impedit explicabo est fuga veniam facere nam
            iste provident.
          </div>
          <div class="issueButtons">
            <button class="sendIssueToManager">
              Wyślij zgłoszenie do menedżera
            </button>
            <button class="deleteIssue">Usuń zgłoszenie</button>
          </div>
        </div>
      </div>
    </main>
  </div>
</template>

<script>
export default {
  data() {
    return {
      serviceAndRepairVisible: true,
      newCarVisible: true,
      issueVisible: true,
    };
  },
};
</script>

<style scoped>
@import "./styles/style.css";
</style>

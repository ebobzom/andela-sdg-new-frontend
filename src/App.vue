<template>
  <div id="app" role="main-app">
    <div class="container" role="container">
      <h1>Covid-19 Estimator</h1>
      <form action="#" method="POST">
          <label for="population">Population</label>
          <input data-population type="text" id="population" placeholder="population" aria-label="population">

          <label for="timeToElapse">Time To Elapse</label>
          <input data-time-to-elapse type="number" id="timeToElapse" placeholder="timeToElapse" aria-label="timeToElapse">

          <label for="reportedCases">Reported Cases</label>
          <input data-reported-cases type="number" id="reportedCases" placeholder="reportedCases" aria-label="reportedCases">

          <label for="totalHospitalBeds">Total Hospital Beds</label>
          <input data-total-hospital-beds type="number" id="totalHospitalBeds" placeholder="totalHospitalBeds" aria-label="totalHospitalBeds">

          <label for="periodType">Period Type</label>
          <select data-period-type name="periodType" id="periodType">
              <option value="days">Days</option>
              <option value="weeks">Weeks</option>
              <option value="months">Months</option>
          </select>
          <button data-go-estimate>Submit</button>
      </form>

    </div>
  </div>
</template>

<script>


export default {
  name: 'App',
  components: {
  }
}
</script>

<style>
body{
    background-color: #f5f5f5;
    font-size: 1.5em;
}

h1{
    text-align: center;
}

form{
    width: 40%;
    margin: 0 auto;
    border: 1px solid grey;
    border-radius: 10px;
}


input, label{
    display: block;
    margin: 4px auto;
    width: 80%;
    height: 30px;
    border-radius: 4px;
}

label{
    padding: 2px;
    margin-top: 2px;
    font-style: italic;
    font-weight: 600;
}
button, select{
    height: 30px;
    border-radius: 4px;
    display: block;
}

label[for='periodType']{
    display: inline-block;
    text-align: center;
    padding: 10px;
}

select{
    text-align: center;
    width: 30%;
    text-align: center;
    margin: 0 auto;
}

button{
    width: 30%;
    margin: 0 auto;
    height: 35px;
    margin-top: 20px;
    background-color: rgb(165, 209, 165);
    font-weight: bold;
}
</style>

import config from "./conf/index.js";

// Implementation of fetch call to fetch all adventure
async function fetchReservations() {
  // TODO: MODULE_RESERVATIONS
  // 1. FETCH Reservations by invoking the REST API and return them

  // fetch operations

  // placeholder for functionality to work in the stubs
  return null;
}

// Implementation to extract city from query params
function getCityFromURL(search) {
  // TODO: MODULE_ADVENTURES
  // 1. Extract the city id from the URL's Param and return it

  // use URLSearchParams to extract the city from city=your cityname
  let city = "bengaluru"; // use URLSearchParams() with window.location.search correctly
  return city;
}

// Implementation of fetch call with parameterized input based on city
async function fetchAdventuresDetails(adventureID) {
  // TODO: MODULE_ADVENTURES
  // 1. Fetch the details of the adventure by making an API call
  let URL = ""; // Define the URL based on adventureID

  let res = await fetch(URL);
  let data = await res.json();

  // placeholder for functionality to work in the stubs
  return data;
}

// Implementation of DOM manipulation to add adventure details to DOM
function addAdventureToDOM(adventure) {
  // TODO: MODULE_ADVENTURES_DETAILS
  // 1. Add the details of the adventure to the HTML DOM

  document.getElementById("put-the-correct-id1").innerHTML = adventure.name;
  document.getElementById("put-the-correct-id2").innerHTML = adventure.subtitle;

  adventure.images.map((image) => {
    let element = document.createElement("div");
    // append element to DOM
  });
}

// Implementation of bootstrap gallery component
function addBootstrapPhotoGallery(images) {
  // TODO: MODULE_ADVENTURES_DETAILS
  // 1. Add the bootstrap carousel to show the adventure images

  document.getElementById("photo-gallery").innerHTML = `
    <div id="carouselExampleIndicators" class="carousel slide" data-ride="carousel">
      <ol class="carousel-indicators">
        ${images.map((_, index) => `<li data-target="#carouselExampleIndicators" data-slide-to="${index}" class="${index === 0 ? 'active' : ''}"></li>`).join('')}
      </ol>
      <div class="carousel-inner">
        ${images.map((image, index) => `
          <div class="carousel-item ${index === 0 ? 'active' : ''}">
            <img src="${image}" class="d-block w-100" alt="Adventure Image">
          </div>`).join('')}
      </div>
      <a class="carousel-control-prev" href="#carouselExampleIndicators" role="button" data-slide="prev">
        <span class="carousel-control-prev-icon" aria-hidden="true"></span>
        <span class="sr-only">Previous</span>
      </a>
      <a class="carousel-control-next" href="#carouselExampleIndicators" role="button" data-slide="next">
        <span class="carousel-control-next-icon" aria-hidden="true"></span>
        <span class="sr-only">Next</span>
      </a>
    </div>`;
}

// Implementation of conditional rendering of DOM based on availability
function conditionalRenderingOfReservationPanel(adventure) {
  // TODO: MODULE_ADVENTURES_DETAILS
  // 1. If the adventure is already reserved, display the sold-out message

  // 1. check if available is true/false from adventure
  // 2. getElementById('')
  // 3. element.style.display = 'none' / 'block'
}

// Implementation of reservation cost calculation based on persons
function calculateReservationCostAndUpdateDOM(adventure, persons) {
  // TODO: MODULE_RESERVATIONS
  // 1. Calculate the cost based on the number of persons and update the reservation-cost field

  // take the cost per head * persons
}

// Implementation of reservation form submission using jQuery
function captureFormSubmitUsingJQuery(adventure) {
  // TODO: MODULE_RESERVATIONS
  // 1. Capture the form details and make a post API call using jQuery to make the reservations
  // 2. If the reservation is successful, show an alert with "Success" and refresh the pages.
  //    If the reservation fails, just show an alert with "fails"

  // submit(
  //   ajax (
  //     success, failure
  //   )
  // )
  $("#myForm").submit(function (event) {
    event.preventDefault(); // preventing default form behavior
    // 1. Serialize form request
    // 2. Ajax to send it to the backend endpoint
    let formData = $(this).serialize();
    $.ajax({
      method: "post",
      url: "some.php",
      data: formData,
      success: function () {},
      error: function () {},
    });
  });
}

// Implementation of success banner after reservation
function showBannerIfAlreadyReserved(adventure) {
  // TODO: MODULE_RESERVATIONS
  // 1. If the user has already reserved this adventure, show the reserved-banner; otherwise, don't

  // check the reserved prop if it's true/false
  // getElementById('')
  // element.style.display = 'none' / 'block'
}

// Implementation of DOM manipulation to add adventures for the given city from the list of adventures
function addAdventureToDOM(adventures) {
  // TODO: MODULE_ADVENTURES
  // 1. Populate the adventure Cards and insert these details into the DOM

  // take out each object (adventure)
  // create HTML necessary
  // Remember to use the correct classes (look up style.css or bootstrap classes)
  // placeHolder for functionality to work in the Stubes
}

// Implementation of filtering by duration which takes in a list of adventures
function filteringByDuration(lists, low, high) {
  // TODO: MODULE_FILTERS
  // 1. Filter adventures based on Duration and return the filtered list

  // go through each list, for each adventure
  // check if duration is within bounds
  return filteredList;
}

// Implementation of filtering by category which takes in a list of adventures, a list of categories to be filtered
function filterByCategory(list, categoryList) {
  // TODO: MODULE_FILTERS
  // 1. Filter adventures based on their Category and return the filtered list

  // through each of adventures in the list
  // see if it belongs in the category as given by categoryList
  return filteredList;
}

// filters object looks like this filters = { duration: "", category: [] };

// Implementation of the combined filter function that covers the following cases:
// 1. Filter by duration only
// 2. Filter by category only
// 3. Filter by duration and category together
function filterFunction(lists, filters) {
  // TODO: MODULE_FILTERS
  // 1. Handle the 3 cases detailed in the comments above the filtered list of adventures
  // 2. Depending on which filters are needed, invoke the filterByDuration() and/or
} 





import config from "./conf/index.js";

// Implementation of fetch call to fetch all adventure
async function fetchReservations() {
  // TODO: MODULE_RESERVATIONS
  // 1. FETCH Reservations by invoking the REST API and return them

  // fetch operations

  // placeholder for functionality to work in the stubs
  return null;
}

// Implementation to extract city from query params
function getCityFromURL(search) {
  // TODO: MODULE_ADVENTURES
  // 1. Extract the city id from the URL's Param and return it

  // use URLSearchParams to extract the city from city=your cityname
  let city = "bengaluru"; // use URLSearchParams() with window.location.search correctly
  return city;
}

// Implementation of fetch call with parameterized input based on city
async function fetchAdventuresDetails(adventureID) {
  // TODO: MODULE_ADVENTURES
  // 1. Fetch the details of the adventure by making an API call
  let URL = ""; // Define the URL based on adventureID

  let res = await fetch(URL);
  let data = await res.json();

  // placeholder for functionality to work in the stubs
  return data;
}

// Implementation of DOM manipulation to add adventure details to DOM
function addAdventureToDOM(adventure) {
  // TODO: MODULE_ADVENTURES_DETAILS
  // 1. Add the details of the adventure to the HTML DOM

  document.getElementById("put-the-correct-id1").innerHTML = adventure.name;
  document.getElementById("put-the-correct-id2").innerHTML = adventure.subtitle;

  adventure.images.map((image) => {
    let element = document.createElement("div");
    // append element to DOM
  });
}

// Implementation of bootstrap gallery component
function addBootstrapPhotoGallery(images) {
  // TODO: MODULE_ADVENTURES_DETAILS
  // 1. Add the bootstrap carousel to show the adventure images

  document.getElementById("photo-gallery").innerHTML = `
    <div id="carouselExampleIndicators" class="carousel slide" data-ride="carousel">
      <ol class="carousel-indicators">
        ${images.map((_, index) => `<li data-target="#carouselExampleIndicators" data-slide-to="${index}" class="${index === 0 ? 'active' : ''}"></li>`).join('')}
      </ol>
      <div class="carousel-inner">
        ${images.map((image, index) => `
          <div class="carousel-item ${index === 0 ? 'active' : ''}">
            <img src="${image}" class="d-block w-100" alt="Adventure Image">
          </div>`).join('')}
      </div>
      <a class="carousel-control-prev" href="#carouselExampleIndicators" role="button" data-slide="prev">
        <span class="carousel-control-prev-icon" aria-hidden="true"></span>
        <span class="sr-only">Previous</span>
      </a>
      <a class="carousel-control-next" href="#carouselExampleIndicators" role="button" data-slide="next">
        <span class="carousel-control-next-icon" aria-hidden="true"></span>
        <span class="sr-only">Next</span>
      </a>
    </div>`;
}

// Implementation of conditional rendering of DOM based on availability
function conditionalRenderingOfReservationPanel(adventure) {
  // TODO: MODULE_ADVENTURES_DETAILS
  // 1. If the adventure is already reserved, display the sold-out message

  // 1. check if available is true/false from adventure
  // 2. getElementById('')
  // 3. element.style.display = 'none' / 'block'
}

// Implementation of reservation cost calculation based on persons
function calculateReservationCostAndUpdateDOM(adventure, persons) {
  // TODO: MODULE_RESERVATIONS
  // 1. Calculate the cost based on the number of persons and update the reservation-cost field

  // take the cost per head * persons
}

// Implementation of reservation form submission using jQuery
function captureFormSubmitUsingJQuery(adventure) {
  // TODO: MODULE_RESERVATIONS
  // 1. Capture the form details and make a post API call using jQuery to make the reservations
  // 2. If the reservation is successful, show an alert with "Success" and refresh the pages.
  //    If the reservation fails, just show an alert with "fails"

  // submit(
  //   ajax (
  //     success, failure
  //   )
  // )
  $("#myForm").submit(function (event) {
    event.preventDefault(); // preventing default form behavior
    // 1. Serialize form request
    // 2. Ajax to send it to the backend endpoint
    let formData = $(this).serialize();
    $.ajax({
      method: "post",
      url: "some.php",
      data: formData,
      success: function () {},
      error: function () {},
    });
  });
}

// Implementation of success banner after reservation
function showBannerIfAlreadyReserved(adventure) {
  // TODO: MODULE_RESERVATIONS
  // 1. If the user has already reserved this adventure, show the reserved-banner; otherwise, don't

  // check the reserved prop if it's true/false
  // getElementById('')
  // element.style.display = 'none' / 'block'
}

// Implementation of DOM manipulation to add adventures for the given city from the list of adventures
function addAdventureToDOM(adventures) {
  // TODO: MODULE_ADVENTURES
  // 1. Populate the adventure Cards and insert these details into the DOM

  // take out each object (adventure)
  // create HTML necessary
  // Remember to use the correct classes (look up style.css or bootstrap classes)
  // placeHolder for functionality to work in the Stubes
}

// Implementation of filtering by duration which takes in a list of adventures
function filteringByDuration(lists, low, high) {
  // TODO: MODULE_FILTERS
  // 1. Filter adventures based on Duration and return the filtered list

  // go through each list, for each adventure
  // check if duration is within bounds
  return filteredList;
}

// Implementation of filtering by category which takes in a list of adventures, a list of categories to be filtered
function filterByCategory(list, categoryList) {
  // TODO: MODULE_FILTERS
  // 1. Filter adventures based on their Category and return the filtered list

  // through each of adventures in the list
  // see if it belongs in the category as given by categoryList
  return filteredList;
}

// filters object looks like this filters = { duration: "", category: [] };

// Implementation of the combined filter function that covers the following cases:
// 1. Filter by duration only
// 2. Filter by category only
// 3. Filter by duration and category together
function filterFunction(lists, filters) {
  // TODO: MODULE_FILTERS
  // 1. Handle the 3 cases detailed in the comments above the filtered list of adventures
  // 2. Depending on which filters are needed, invoke the filterByDuration() and/or
} 






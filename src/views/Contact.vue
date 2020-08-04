<template>
<section class="appointment v2">
      <div class="appointment-wrap">
        <figure>
          <img src="images/appointment-img.jpg" alt="">
        </figure>
        <div class="appointment-form">
          <form action="#">
            <div class="form-field half-width">
              <input type="text" placeholder="NAME" required>
              <input type="email" placeholder="Email address" required>
            </div>
            <div class="form-field half-width">
              <div class="select-field">
                <select>
                  <option>Select service</option>
                  <option>Select service 1</option>
                </select>
              </div>
              <input type="tel" placeholder="Phone numer">
            </div>
            <div class="form-field half-width">
              <input type="date" placeholder="date">
              <input type="time" placeholder="time">
            </div>
            <div class="form-field">
              <textarea name="notes" placeholder="Your notes"></textarea>
            </div>
            <button class="btn btn-round">Make an Appointment</button>
          </form>
        </div>
      </div>
    </section>
</template>

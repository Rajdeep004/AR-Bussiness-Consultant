<script>
  import { Link } from "svelte-navigator";
</script>

<footer
  class="sm:w-full bg-gradient-to-b sm:bg-gradient-to-r from-[#006FF2] to-[#004391] text-white"
>
  <div class="flex flex-col lg:flex-row w-full p-8 gap-6">
    <div class="w-full">
      <div class="border-4 rounded-full w-max scale-75">
        <Link to="/" >
          <img 
            src="AR white logo.svg" 
            alt="AR Secondary Logo"
            class="p-6 "
          >
        </Link> 
      </div>
      <h3 class="text-xl font-semibold">AR Business Consultant</h3>
    </div>
    <div class="w-full">
      <h4 class="text-xl font-semibold">Pages</h4>
      <ul class="flex flex-col">
        <Link to="/" >Home</Link>
        <Link to="/about">About Us</Link>
        <Link to="/services">Services</Link>
        <Link to="/connect">Connect</Link>
      </ul>
    </div>
    <div class="w-full">
      <div class="w-full">
        <h4 class="text-xl font-semibold">Connect</h4>
        <ul class="flex flex-col">
          <a target="_blank" href="tel:+44 7466984571"><svg class="inline-flex" xmlns="http://www.w3.org/2000/svg" width="24" height="32" viewBox="0 0 24 24"><path fill="#ffffff" d="M19 11.95q0-2.925-2.037-4.962T12 4.95v-2q1.875 0 3.513.713t2.85 1.925q1.212 1.212 1.925 2.85T21 11.95zm-4 0q0-1.25-.875-2.125T12 8.95v-2q2.075 0 3.538 1.463T17 11.95zM19.95 21q-3.125 0-6.175-1.362t-5.55-3.863q-2.5-2.5-3.862-5.55T3 4.05q0-.45.3-.75t.75-.3H8.1q.35 0 .625.238t.325.562l.65 3.5q.05.4-.025.675T9.4 8.45L6.975 10.9q.5.925 1.187 1.787t1.513 1.663q.775.775 1.625 1.438T13.1 17l2.35-2.35q.225-.225.588-.337t.712-.063l3.45.7q.35.1.575.363T21 15.9v4.05q0 .45-.3.75t-.75.3"/></svg> <span>+44 7466984571</span></a>
          <a target="_blank" href="mailto:info.arbusinessconsultant@gmail.com"><svg class="inline-flex" xmlns="http://www.w3.org/2000/svg" width="24" height="32" viewBox="0 0 24 24"><path fill="#ffffff" d="M4 20q-.825 0-1.412-.587T2 18V6q0-.825.588-1.412T4 4h16q.825 0 1.413.588T22 6v12q0 .825-.587 1.413T20 20zm8-7.175q.125 0 .263-.038t.262-.112L19.6 8.25q.2-.125.3-.312t.1-.413q0-.5-.425-.75T18.7 6.8L12 11L5.3 6.8q-.45-.275-.875-.012T4 7.525q0 .25.1.438t.3.287l7.075 4.425q.125.075.263.113t.262.037"/></svg> <span>info.arbusinessconsultant@gmail.com</span></a>
          <a target="_blank" href="https://maps.app.goo.gl/pXRBKw4SnaFDeiXy6"><svg class="inline-flex" xmlns="http://www.w3.org/2000/svg" width="24" height="32" viewBox="0 0 24 24"><path fill="#ffffff" d="M12 2C8.13 2 5 5.13 5 9c0 5.25 7 13 7 13s7-7.75 7-13c0-3.87-3.13-7-7-7m0 9.5a2.5 2.5 0 0 1 0-5a2.5 2.5 0 0 1 0 5"/></svg> <span>57 Oakwood Crescent, Greenford, England, UB6 0RF</span></a>
        </ul>
      </div>
    </div>
    <div class="w-full">
      <a href="https://www.linkedin.com/company/a-r-business-consultant-limited" target="_blank"><h4 class="text-xl font-semibold">Social Media</h4></a>
      <ul class="flex flex-col">
        <li>Linkedin</li>
      </ul>
    </div>
  </div>
  <h5 class="text-center text-lg font-bold mb-4">
    Developed by The Coding Devotees
  </h5>
</footer>

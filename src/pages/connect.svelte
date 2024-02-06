<script>
  import Footer from "./Footer.svelte";
  import Navbar from "./Navbar.svelte";
</script>

<Navbar />
<section
  id="quotation"
  class="container mx-auto lg:w-1/2 lg:max-h-screen my-12 flex flex-col lg:items-center gap-6"
>
  <h1 class="text-center text-4xl lg:text-5xl font-bold">Get a quotation ?</h1>
  <div>
    <form action="https://formsubmit.io/send/info.arbusinessconsultant@gmail.com" method="post">
      <div class="flex flex-col lg:flex-row gap-4 lg:gap-12">
        <div class="lft-div flex flex-col gap-4 lg:w-1/2 flex-grow-0">
          <input
            type="text"
            name="Name"
            placeholder="Name"
            class="p-2 border border-gray-400 rounded-lg lg:max-w-xs"
          />
          <input
            type="email"
            name="Email"
            placeholder="Email"
            class="p-2 border border-gray-400 rounded-lg lg:max-w-xs"
          />
          <input
            type="tel"
            name="Phone"
            placeholder="Phone"
            class="p-2 border border-gray-400 rounded-lg lg:max-w-xs lg:hidden"
          />
          <div class="radio-btn">
            <h3 class="font-bold text-lg">Type of organisation?</h3>
            <div class="option">
              <div class="opt1">
                <input type="radio" id="company" name="option" />
                <label for="company">Company</label>
              </div>
              <div class="opt2">
                <input type="radio" id="soletrader" name="option" />
                <label for="soletrader">Sole Trader</label>
              </div>
              <div class="opt3">
                <input type="radio" id="individual" name="option" />
                <label for="individual">Individual</label>
              </div>
              <div class="opt4">
                <input type="radio" id="partnership" name="option" />
                <label for="partnership">Partnership</label>
              </div>
            </div>
          </div>
          <input
            type="text"
            name="Are you VAT registered?"
            placeholder="Are you VAT registered?"
            class="p-2 border border-gray-400 rounded-lg lg:max-w-xs"
          />
          <input
            type="text"
            name="Approximate turnover?"
            placeholder="Approximate turnover?"
            class="p-2 border border-gray-400 rounded-lg lg:max-w-xs"
          />
          <input
            type="text"
            name="Number of employees?"
            placeholder="Number of employees?"
            class="p-2 border border-gray-400 rounded-lg lg:max-w-xs"
          />
        </div>
        <div class="rght-div flex flex-col gap-4 lg:w-1/2 flex-grow-0">
          <input
            type="tel"
            name="Phone"
            placeholder="Phone"
            class="p-2 border border-gray-400 rounded-lg max-w-xs hidden lg:block"
          />
          <div class="radio-btn">
            <h3 class="font-bold text-lg">Services intrest in?</h3>
            <div class="option">
              <div class="opt1">
                <input type="radio" id="account" name="option1" />
                <label for="account">Accounts preparation</label>
              </div>
              <div class="opt2">
                <input type="radio" id="tax" name="option1" />
                <label for="tax">Tax return</label>
              </div>
              <div class="opt3">
                <input type="radio" id="vat" name="option1" />
                <label for="vat">VAT filings</label>
              </div>
              <div class="opt4">
                <input type="radio" id="payroll" name="option1" />
                <label for="payroll">Payroll preparation</label>
              </div>
              <div class="opt5">
                <input type="radio" id="book" name="option1" />
                <label for="book">Bookkeeping</label>
              </div>
              <div class="opt6">
                <input type="radio" id="else" name="option1" />
                <label for="else">Something else</label>
              </div>
            </div>
          </div>
          <textarea
            name="Message"
            rows="6"
            placeholder="Any other comments"
            class="p-2 border border-gray-400 rounded-lg"
          ></textarea>
        </div>
      </div>
      <button
        type="submit"
        class="w-full py-3 mt-6 mx-auto text-center rounded-full transition bg-blue-600 hover:bg-blue-700 active:bg-blue-700 focus:bg-blue-600"
        ><span class="block text-white font-semibold text-sm">Submit Quotation</span
        ></button
      >
    </form>
  </div>
</section>
<Footer />

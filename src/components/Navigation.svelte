<script>
    let navState = 'hidden';

    const toggleNavBar = () =>{
        if(navState == 'hidden'){
            navState = '';
        }
        else{
            navState = 'hidden';
        }
    }
</script>

<!-- #navigation container -->

<nav class="bg-white border-gray-200 fixed w-full top-0 p-4 px-2 sm:px-4 rounded ">
    <div class="container p-2 flex flex-wrap items-center justify-between mx-auto">
      <a href="/" class="flex items-center">
          <img src="https://flowbite.com/docs/images/logo.svg" class="h-6 mr-3 sm:h-9" alt="Flowbite Logo" />
          <span class="self-center text-xl font-semibold whitespace-nowrap text-gray-700">FINMAAT</span>
      </a>
      <button on:click={toggleNavBar}  type="button" class="inline-flex items-center p-2 ml-3 text-sm text-gray-500 rounded-lg md:hidden hover:bg-gray-100 focus:outline-none focus:ring-2 focus:ring-gray-200 dark:text-gray-400 dark:hover:bg-gray-700 dark:focus:ring-gray-600" aria-controls="navbar-default" aria-expanded="false">
        <span class="sr-only">Open main menu</span>
        <svg class="w-6 h-6" aria-hidden="true" fill="currentColor" viewBox="0 0 20 20" xmlns="http://www.w3.org/2000/svg"><path fill-rule="evenodd" d="M3 5a1 1 0 011-1h12a1 1 0 110 2H4a1 1 0 01-1-1zM3 10a1 1 0 011-1h12a1 1 0 110 2H4a1 1 0 01-1-1zM3 15a1 1 0 011-1h12a1 1 0 110 2H4a1 1 0 01-1-1z" clip-rule="evenodd"></path></svg>
      </button>
      <div class="{navState} delay-75 w-full md:block md:w-auto" id="navbar-default">
        <ul class="flex flex-col p-4 mt-4 border border-gray-200 rounded-lg bg-gray-100 md:flex-row md:space-x-8 md:mt-0 md:text-sm md:font-medium md:border-0 md:bg-white ">
          <li>
            <a href="/" class="block py-4 pl-3  text-base pr-4 text-white p-2 bg-indigo-700 rounded md:bg-transparent md:text-blue-700 md:p-0" aria-current="page">Home</a>
          </li>
          <li>
            <a href="/About" class="block py-4 text-base lg:mt-0 md:mt-0 mt-2  pl-3 pr-4 text-gray-700 rounded hover:bg-indigo-600 hover:text-white md:hover:bg-transparent md:border-0 md:hover:text-blue-700 md:p-0">About</a>
          </li>
          <li>
            <a href="/Trainings" class="block text-base  py-4 pl-3 pr-4 text-gray-700 rounded hover:bg-indigo-600 hover:text-white md:hover:bg-transparent md:border-0 md:hover:text-blue-700 md:p-0">Services</a>
          </li>
          <li>
            <a href="/Contact Us" class="block text-base  py-4 pl-3 pr-4 text-gray-700 rounded hover:bg-indigo-600 hover:text-white md:hover:bg-transparent md:border-0 md:hover:text-blue-700 md:p-0">Contact</a>
          </li>
        </ul>
      </div>
    </div>
  </nav>
  
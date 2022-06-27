- 👋 Hi, I’m @vinrib
- 👀 I’m interested in ...
- 🌱 I’m currently learning ...
- 💞️ I’m looking to collaborate on ...
- 📫 How to reach me 

<!---
vinrib/vinrib is a ✨ special ✨ repository because its `README.md` (this file) appears on your GitHub profile.
You can click the Preview link to take a look at your changes.
--->
<!DOCTYPE html>
<html lang="en">

<head>
    <meta charset="UTF-8">
    <meta http-equiv="X-UA-Compatible" content="IE=edge">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <script src="https://cdn.tailwindcss.com"></script>
    <style>
        #btn-press {
            position: relative;
            top: 0;
            background: #0928f2;
            color: #fff;
            box-shadow: 0px 6px rgb(255, 190, 186);
            transition: 0.05s !important;
        }

        #btn-press:hover {
            top: 3px;
            box-shadow: 0px 3px rgb(146, 78, 255);

        }

        #btn-press {
            top: 6px;
            box-shadow: 0px 0px rgb(255, 143, 123);
        }

        #Title {
            font-family: 'Segoe UI', Tahoma, Geneva, Verdana, sans-serif;
            font-size: 45px;
            text-shadow: 2px 2px 2px #ababab;
            font-weight: 500;
        }

        #Title::selection {
            background-color: beige;
        }

        #icon-card {
            width: 64px;
            height: 64px;
        }

        .slider {
            width: 200px;
            height: 400px;
            position: relative;
            overflow: hidden;
        }

        .slide-ana {
            height: 360px;
        }

        .slide-ana>div {
            width: 100%;
            height: 100%;
            position: absolute;
            transition: all 0.7s;
        }

        @media (min-width: 200px) and (max-width: 639px) {
            .slider {
                height: 300px;
                width: 170px;
            }
        }


        .card {
            width: 220px;
            height: 321px;
            background: #fff;
            border-top-right-radius: 10px;
            overflow: hidden;
            display: flex;
            flex-direction: column;
            justify-content: center;
            align-items: center;
            position: relative;
            box-shadow: 0 14px 26px rgba(0, 0, 0, 0.04);
            transition: all 0.3s ease-out;
            text-decoration: none;
        }

        .card:hover {
            transform: translateY(-5px) scale(1.005) translateZ(0);
            box-shadow: 0 24px 36px rgba(0, 0, 0, 0.11),
                0 24px 46px var(--box-shadow-color);
        }

        .card:hover .overlay {
            transform: scale(4) translateZ(0);
        }

        .card:hover .circle {
            border-color: var(--bg-color-light);
            background: var(--bg-color);
        }

        .card:hover .circle:after {
            background: var(--bg-color-light);
        }

        .card:hover p {
            color: var(--text-color-hover);
        }

        .card:active {
            transform: scale(1) translateZ(0);
            box-shadow: 0 15px 24px rgba(0, 0, 0, 0.11),
                0 15px 24px var(--box-shadow-color);
        }

        .card p {
            font-size: 17px;
            color: #4C5656;
            margin-top: 30px;
            z-index: 1000;
            transition: color 0.3s ease-out;
        }

        .circle {
            width: 131px;
            height: 131px;
            border-radius: 50%;
            background: #fff;
            border: 2px solid var(--bg-color);
            display: flex;
            justify-content: center;
            align-items: center;
            position: relative;
            z-index: 1;
            transition: all 0.3s ease-out;
        }

        .circle:after {
            content: "";
            width: 118px;
            height: 118px;
            display: block;
            position: absolute;
            background: var(--bg-color);
            border-radius: 50%;
            top: 7px;
            left: 7px;
            transition: opacity 0.3s ease-out;
        }

        .circle svg {
            z-index: 10000;
            transform: translateZ(0);
        }

        .overlay {
            width: 118px;
            position: absolute;
            height: 118px;
            border-radius: 50%;
            background: var(--bg-color);
            top: 70px;
            left: 50px;
            z-index: 0;
            transition: transform 0.3s ease-out;
        }

        h1 {
            font-family: system-ui, sans-serif;
        }
    </style>
    <title>Wiress</title>
</head>

<body>

    <div class="h-full w-full">
        <!-- Code block starts -->
        <nav role="navigation" class="bg-white shadow xl:block hidden">
            <div class="max-w-7xlmx-auto container px- py-3 xl:py-0">
                <div class="flex items-center justify-between">
                    <div class="inset-y-0 left-0 flex items-center xl:hidden">
                        <div
                            class="inline-flex items-center justify-center p-2 rounded-md text-gray-700 hover:text-gray-100 focus:outline-none transition duration-150 ease-in-out">
                            <div class="visible xl:hidden">
                                <ul
                                    class="p-2 border-r bg-white absolute rounded left-0 right-0 shadow mt-8 md:mt-8 hidden">
                                    <li
                                        class="flex xl:hidden cursor-pointer text-gray-600 text-sm leading-3 tracking-normal mt-2 py-2 hover:text-indigo-700 focus:text-indigo-700 focus:outline-none">
                                        <div class="flex items-center">
                                            <svg xmlns="http://www.w3.org/2000/svg"
                                                class="icon icon-tabler icon-tabler-grid" width="20" height="20"
                                                viewBox="0 0 24 24" stroke-width="1.5" stroke="currentColor" fill="none"
                                                stroke-linecap="round" stroke-linejoin="round">
                                                <path stroke="none" d="M0 0h24v24H0z"></path>
                                                <rect x="4" y="4" width="6" height="6" rx="1"></rect>
                                                <rect x="14" y="4" width="6" height="6" rx="1"></rect>
                                                <rect x="4" y="14" width="6" height="6" rx="1"></rect>
                                                <rect x="14" y="14" width="6" height="6" rx="1"></rect>
                                            </svg>
                                            <span class="ml-2 font-bold">Produtos</span>
                                        </div>
                                    </li>
                                    <li class="flex xl:hidden flex-col cursor-pointer text-gray-600 text-sm leading-3 tracking-normal py-2 hover:text-indigo-700 focus:text-indigo-700 focus:outline-none flex justify-center"
                                        onclick="dropdownHandler(this)">
                                        <div class="flex items-center">
                                            <svg xmlns="http://www.w3.org/2000/svg"
                                                class="icon icon-tabler icon-tabler-puzzle" width="20" height="20"
                                                viewBox="0 0 24 24" stroke-width="1.5" stroke="currentColor" fill="none"
                                                stroke-linecap="round" stroke-linejoin="round">
                                                <path stroke="none" d="M0 0h24v24H0z"></path>
                                                <path
                                                    d="M4 7h3a1 1 0 0 0 1 -1v-1a2 2 0 0 1 4 0v1a1 1 0 0 0 1 1h3a1 1 0 0 1 1 1v3a1 1 0 0 0 1 1h1a2 2 0 0 1 0 4h-1a1 1 0 0 0 -1 1v3a1 1 0 0 1 -1 1h-3a1 1 0 0 1 -1 -1v-1a2 2 0 0 0 -4 0v1a1 1 0 0 1 -1 1h-3a1 1 0 0 1 -1 -1v-3a1 1 0 0 1 1 -1h1a2 2 0 0 0 0 -4h-1a1 1 0 0 1 -1 -1v-3a1 1 0 0 1 1 -1">
                                                </path>
                                            </svg>
                                            <span class="ml-2 font-bold">APIs</span>
                                        </div>
                                    </li>
                                    <li
                                        class="flex xl:hidden cursor-pointer text-gray-600 text-sm leading-3 tracking-normal py-2 hover:text-indigo-700 flex items-center focus:text-indigo-700 focus:outline-none">
                                        <svg xmlns="http://www.w3.org/2000/svg"
                                            class="icon icon-tabler icon-tabler-compass" width="20" height="20"
                                            viewBox="0 0 24 24" stroke-width="1.5" stroke="currentColor" fill="none"
                                            stroke-linecap="round" stroke-linejoin="round">
                                            <path stroke="none" d="M0 0h24v24H0z"></path>
                                            <polyline points="8 16 10 10 16 8 14 14 8 16"></polyline>
                                            <circle cx="12" cy="12" r="9"></circle>
                                        </svg>
                                        <span class="ml-2 font-bold">Dashboard</span>
                                    </li>
                                    <li
                                        class="border-b border-gray-300 flex xl:hidden cursor-pointer text-gray-600 text-sm leading-3 tracking-normal pt-2 pb-4 hover:text-indigo-700 flex items-center focus:text-indigo-700 focus:outline-none">
                                        <svg xmlns="http://www.w3.org/2000/svg"
                                            class="icon icon-tabler icon-tabler-code" width="20" height="20"
                                            viewBox="0 0 24 24" stroke-width="1.5" stroke="currentColor" fill="none"
                                            stroke-linecap="round" stroke-linejoin="round">
                                            <path stroke="none" d="M0 0h24v24H0z"></path>
                                            <polyline points="7 8 3 12 7 16"></polyline>
                                            <polyline points="17 8 21 12 17 16"></polyline>
                                            <line x1="14" y1="4" x2="10" y2="20"></line>
                                        </svg>
                                        <span class="ml-2 font-bold">Documentação</span>
                                    </li>
                                    <li
                                        class="cursor-pointer text-gray-600 text-sm leading-3 tracking-normal mt-2 py-2 hover:text-indigo-700 flex items-center focus:text-indigo-700 focus:outline-none">
                                        <div class="flex items-center">
                                            <div
                                                class="w-12 cursor-pointer flex text-sm border-2 border-transparent rounded focus:outline-none focus:border-white transition duration-150 ease-in-out">
                                                <img class="rounded h-10 w-10 object-cover" src="user.png" alt="logo" />
                                            </div>
                                            <p class="text-sm ml-2 cursor-pointer">Jane Doe</p>
                                            <div class="sm:ml-2 text-white relative">
                                                <svg xmlns="http://www.w3.org/2000/svg"
                                                    class="icon icon-tabler icon-tabler-chevron-down cursor-pointer"
                                                    width="20" height="20" viewBox="0 0 24 24" stroke-width="1.5"
                                                    stroke="currentColor" fill="none" stroke-linecap="round"
                                                    stroke-linejoin="round">
                                                    <path stroke="none" d="M0 0h24v24H0z"></path>
                                                    <polyline points="6 9 12 15 18 9"></polyline>
                                                </svg>
                                            </div>
                                        </div>
                                    </li>
                                    <li
                                        class="cursor-pointer text-gray-600 text-sm leading-3 tracking-normal py-2 hover:text-indigo-700 focus:text-indigo-700 focus:outline-none">
                                        <div class="flex items-center">
                                            <svg xmlns="http://www.w3.org/2000/svg"
                                                class="icon icon-tabler icon-tabler-user" width="20" height="20"
                                                viewBox="0 0 24 24" stroke-width="1.5" stroke="currentColor" fill="none"
                                                stroke-linecap="round" stroke-linejoin="round">
                                                <path stroke="none" d="M0 0h24v24H0z" />
                                                <circle cx="12" cy="7" r="4" />
                                                <path d="M6 21v-2a4 4 0 0 1 4 -4h4a4 4 0 0 1 4 4v2" />
                                            </svg>
                                            <span class="ml-2">Profile</span>
                                        </div>
                                    </li>
                                </ul>
                                <img class="show-m-menu icon icon-tabler icon-tabler-menu"
                                    onclick="MenuHandler(this,true)"
                                    src="https://tuk-cdn.s3.amazonaws.com/can-uploader/light-with-button-svg2.svg"
                                    alt="icon" />
                            </div>
                            <div class="hidden close-m-menu text-gray-700" onclick="MenuHandler(this,false)">
                                <img src="https://tuk-cdn.s3.amazonaws.com/can-uploader/light-with-button-svg1.svg"
                                    alt="icon-2" />
                            </div>
                        </div>
                    </div>
                    <button
                        class="px-20 focus:outline-none focus:ring-2 focus:ring-offset-2 focus:ring-indigo-700 rounded-md flex w-full sm:w-auto items-center sm:items-stretch justify-end sm:justify-start">
                        <div class="flex items-center">
                            <img src="https://tuk-cdn.s3.amazonaws.com/can-uploader/light-with-button-svg3.svg"
                                alt="logo" class="h-16 w-16" />
                            <h2 class="hidden sm:block text-base text-2xl text-gray-700 font-bold leading-normal px-3">
                                Wiress</h2>
                        </div>
                    </button>
                    <div class="flex">
                        <div class="hidden xl:flex md:mr-6 xl:mr-16">
                            <a href="javascript: void(0)"
                                class="focus:text-indigo-700 border-b-2 border-transparent focus:border-indigo-700 flex px-5 items-center py-6 text-sm leading-5 text-gray-700 hover:bg-gray-100 focus:bg-gray-100 focus:outline-none transition duration-150 ease-in-out">
                                <span class="mr-2">
                                    <img class="icon icon-tabler icon-tabler-grid"
                                        src="https://tuk-cdn.s3.amazonaws.com/can-uploader/light-with-button-svg4.svg"
                                        alt="produtos" />
                                </span>
                                <button id="dropdownNavbarLink" data-dropdown-toggle="dropdownNavbar"
                                    class="flex items-center justify-between w-full py-2 pl-3 pr-4 font-medium text-gray-700 border-b border-gray-100 hover:bg-gray-50 md:hover:bg-transparent md:border-0 md:hover:text-blue-700 md:p-0 md:w-auto md:dark:hover:bg-transparent">Produtos
                                    <svg class="w-4 h-4 ml-1" fill="currentColor" viewBox="0 0 20 20"
                                        xmlns="http://www.w3.org/2000/svg">
                                        <path fill-rule="evenodd"
                                            d="M5.293 7.293a1 1 0 011.414 0L10 10.586l3.293-3.293a1 1 0 111.414 1.414l-4 4a1 1 0 01-1.414 0l-4-4a1 1 0 010-1.414z"
                                            clip-rule="evenodd"></path>
                                    </svg></button>
                                <!-- Dropdown menu -->
                                <div id="dropdownNavbar"
                                    class="z-10 hidden bg-white divide-y divide-gray-100 rounded shadow w-44 dark:bg-gray-700 dark:divide-gray-600">
                                    <ul class="py-1 text-sm text-gray-700 dark:text-gray-400"
                                        aria-labelledby="dropdownLargeButton">
                                        <li>
                                            <a href="#"
                                                class="block px-4 py-2 hover:bg-gray-100 dark:hover:bg-gray-600 dark:hover:text-white">Dashboard</a>
                                        </li>
                                        <li>
                                            <a href="#"
                                                class="block px-4 py-2 hover:bg-gray-100 dark:hover:bg-gray-600 dark:hover:text-white">Settings</a>
                                        </li>
                                        <li>
                                            <a href="#"
                                                class="block px-4 py-2 hover:bg-gray-100 dark:hover:bg-gray-600 dark:hover:text-white">Earnings</a>
                                        </li>
                                    </ul>
                                    <div class="py-1">
                                        <a href="#"
                                            class="block px-4 py-2 text-sm text-gray-700 hover:bg-gray-100 dark:hover:bg-gray-600 dark:text-gray-400 dark:hover:text-white">Sign
                                            out</a>
                                    </div>
                                </div>
                                <a href="javascript: void(0)"
                                    class="focus:text-indigo-700 border-b-2 border-transparent focus:border-indigo-700 flex px-5 items-center py-6 text-sm leading-5 text-gray-700 hover:bg-gray-100 focus:bg-gray-100 focus:outline-none transition duration-150 ease-in-out">
                                    <span class="mr-2">
                                        <img class="icon icon-tabler icon-tabler-puzzle"
                                            src="https://tuk-cdn.s3.amazonaws.com/can-uploader/light-with-button-svg5.svg"
                                            alt="APIs" />
                                    </span>
                                    APIs
                                </a>
                                <a href="javascript: void(0)"
                                    class="focus:text-indigo-700 border-b-2 border-transparent focus:border-indigo-700 flex px-5 items-center py-6 text-sm leading-5 text-gray-700 hover:bg-gray-100 focus:bg-gray-100 focus:outline-none transition duration-150 ease-in-out">
                                    <span class="mr-2">
                                        <img class="icon icon-tabler icon-tabler-compass"
                                            src="https://tuk-cdn.s3.amazonaws.com/can-uploader/light-with-button-svg6.svg"
                                            alt="performance" />
                                    </span>
                                    Dashboard
                                </a>
                                <a href="javascript: void(0)"
                                    class="focus:text-indigo-700 border-b-2 border-transparent focus:border-indigo-700 flex px-5 items-center py-6 text-sm leading-5 text-gray-700 hover:bg-gray-100 focus:bg-gray-100 focus:outline-none transition duration-150 ease-in-out">
                                    <span class="mr-2">
                                        <img class="icon icon-tabler icon-tabler-code"
                                            src="https://tuk-cdn.s3.amazonaws.com/can-uploader/light-with-button-svg7.svg"
                                            alt="deliverables" />
                                    </span>
                                    Documentação
                                </a>
                        </div>
                        <div class="hidden xl:flex items-center">
                            <div class="relative md:mr-6 my-2">
                                <button
                                    class="bg-transparent hover:bg-gray-200 text-indigo-700 font-semibold hover:indigo-700 py-2 px-4 border border-indigo-700 hover:border-indigo-700 rounded transition duration-300">
                                    Comece</button>
                                <button
                                    class="bg-indigo-700 hover:bg-transparent text-white font-semibold hover:text-indigo-700 py-2 px-4 border border-transparent hover:border-indigo-700 rounded transition duration-300">
                                    Entrar</button>
                            </div>
                            <div class="ml-6 relative">
                                <button aria-label="dropdown"
                                    class="focus:outline-none border-b-2 border-transparent focus:border-indigo-700 py-3
                                    focus:text-indigo-700 text-gray-600 hover:text-indigo-700 flex items-center relative"
                                    onclick="dropdownHandler(this)">
                                    <ul
                                        class="p-2 w-40 border-r bg-white absolute rounded right-0 shadow top-0 mt-16 hidden">
                                        <li
                                            class="cursor-pointer text-gray-600 text-sm leading-3 tracking-normal py-2 hover:text-indigo-700 focus:text-indigo-700 focus:outline-none">
                                            <a href=""
                                                class="foc us:underline focus:text-indigo-700 focus:outline-none flex items-center">
                                                <svg xmlns="http://www.w3.org/2000/svg"
                                                    class="icon icon-tabler icon-tabler-user" width="18" height="18"
                                                    viewBox="0 0 24 24" stroke-width="1.5" stroke="currentColor"
                                                    fill="none" stroke-linecap="round" stroke-linejoin="round">
                                                    <path stroke="none" d="M0 0h24v24H0z" />
                                                    <circle cx="12" cy="7" r="4" />
                                                    <path d="M6 21v-2a4 4 0 0 1 4 -4h4a4 4 0 0 1 4 4v2" />
                                                </svg>
                                                <span class="ml-2">My Profile</span>
                                            </a>
                                        </li>
                                        <li
                                            class="cursor-pointer text-gray-600 text-sm leading-3 tracking-normal mt-2 py-2 hover:text-indigo-700 focus:text-indigo-700 focus:outline-none flex items-center">
                                            <a href="javascript:void(0)"
                                                class="focus:underline focus:text-indigo-700 focus:outline-none flex items-center">
                                                <svg xmlns="http://www.w3.org/2000/svg"
                                                    class="icon icon-tabler icon-tabler-help" width="20" height="20"
                                                    viewBox="0 0 24 24" stroke-width="1.5" stroke="currentColor"
                                                    fill="none" stroke-linecap="round" stroke-linejoin="round">
                                                    <path stroke="none" d="M0 0h24v24H0z" />
                                                    <circle cx="12" cy="12" r="9" />
                                                    <line x1="12" y1="17" x2="12" y2="17.01" />
                                                    <path d="M12 13.5a1.5 1.5 0 0 1 1 -1.5a2.6 2.6 0 1 0 -3 -4" />
                                                </svg>
                                                <span class="ml-2">Help Center</span>
                                            </a>
                                        </li>
                                        <li
                                            class="cursor-pointer text-gray-600 text-sm leading-3 tracking-normal mt-2 py-2 hover:text-indigo-700 flex items-center focus:text-indigo-700 focus:outline-none">
                                            <a href="javascript:void(0)"
                                                class="focus:underline focus:text-indigo-700 focus:outline-none flex items-center">
                                                <svg xmlns="http://www.w3.org/2000/svg"
                                                    class="icon icon-tabler icon-tabler-settings" width="20" height="20"
                                                    viewBox="0 0 24 24" stroke-width="1.5" stroke="currentColor"
                                                    fill="none" stroke-linecap="round" stroke-linejoin="round">
                                                    <path stroke="none" d="M0 0h24v24H0z" />
                                                    <path
                                                        d="M10.325 4.317c.426-1.756 2.924-1.756 3.35 0a1.724 1.724 0 0 0 2.573 1.066c1.543-.94 3.31.826 2.37 2.37a1.724 1.724 0 0 0 1.065 2.572c1.756.426 1.756 2.924 0 3.35a1.724 1.724 0 0 0 -1.066 2.573c.94 1.543-.826 3.31-2.37 2.37a1.724 1.724 0 0 0 -2.572 1.065c-.426 1.756-2.924 1.756-3.35 0a1.724 1.724 0 0 0 -2.573 -1.066c-1.543.94-3.31-.826-2.37-2.37a1.724 1.724 0 0 0 -1.065 -2.572c-1.756-.426-1.756-2.924 0-3.35a1.724 1.724 0 0 0 1.066 -2.573c-.94-1.543.826-3.31 2.37-2.37.996.608 2.296.07 2.572-1.065z" />
                                                    <circle cx="12" cy="12" r="3" />
                                                </svg>
                                                <span class="ml-2">Account Settings</span>
                                            </a>
                                        </li>
                                    </ul>
                                    <div
                                        class="cursor-pointer flex text-sm border-2 border-transparent rounded-full focus:outline-none focus:border-white transition duration-150 ease-in-out">
                                        <img class="rounded-full h-10 w-10 object-cover" src="user.png"
                                            title="profile icons" alt="logo" />
                                    </div>
                                    <div class="ml-2 ">
                                        <img class="icon icon-tabler icon-tabler-chevron-down cursor-pointer"
                                            src="https://tuk-cdn.s3.amazonaws.com/can-uploader/light-with-button-svg8.svg"
                                            alt="chevron down" />
                                    </div>
                                </button>
                            </div>
                        </div>
                    </div>
                </div>
            </div>
        </nav>
        <nav>
            <div class="py-4 px-6 w-full flex xl:hidden justify-between items-center bg-white fixed top-0 z-40">
                <div aria-label="logo" role="img" tabindex="0" class="focus:outline-none w-24">
                    <img src="https://tuk-cdn.s3.amazonaws.com/can-uploader/light-with-button-svg9.svg" alt="logo" />
                </div>
                <div class="flex items-center">
                    <div class="relative mr-6">
                        <button
                            class="bg-transparent hover:bg-blue-500 text-blue-700 font-semibold hover:text-white py-2 px-4 border border-blue-500 hover:border-transparent rounded">Comece</button>
                    </div>
                    <button id="menu" aria-label="open menu"
                        class="focus:outline-none focus:ring-2 focus:ring-gray-600 rounded-md text-gray-800"
                        onclick="sidebarHandler(true)">
                        <img class="icon icon-tabler icon-tabler-menu-2"
                            src="https://tuk-cdn.s3.amazonaws.com/can-uploader/light-with-button-svg10.svg"
                            alt="menu" />
                    </button>
                </div>
            </div>
            <!--Mobile responsive sidebar-->
            <div class="absolute w-full h-full transform -translate-x-full z-40 xl:hidden" id="mobile-nav">
                <div class="bg-gray-800 opacity-50 w-full h-full" onclick="sidebarHandler(false)"></div>
                <div
                    class="w-64 z-40 fixed overflow-y-auto z-40 top-0 bg-white shadow h-full flex-col justify-between xl:hidden pb-4 transition duration-150 ease-in-out">
                    <div class="px-6 h-full">
                        <div class="flex flex-col justify-between h-full w-full">

                            <div>
                                <!--Icones e menu-->
                                <div class="mt-6 flex w-full items-center justify-between">
                                    <div class="flex items-center justify-between w-full">
                                        <div class="flex items-center">
                                            <img src="https://tuk-cdn.s3.amazonaws.com/can-uploader/light-with-button-svg9.svg"
                                                alt="logo" />
                                            <p tabindex="0"
                                                class="focus:outline-none text-base md:text-2xl text-gray-800 ml-3">
                                                Wiress</p>
                                        </div>
                                        <button id="cross" aria-label="close menu"
                                            class="focus:outline-none focus:ring-2 rounded-md text-gray-800"
                                            onclick="sidebarHandler(false)">
                                            <img class="icon icon-tabler icon-tabler-x"
                                                src="https://tuk-cdn.s3.amazonaws.com/can-uploader/light-with-button-svg11.svg"
                                                alt="cross" />
                                        </button>
                                    </div>
                                </div>
                                <ul class="f-m-m">
                                    <li>
                                        <a class="cursor-pointer">
                                            <div class="text-gray-800 pt-10">
                                                <div class="flex items-center">
                                                    <div class="w-6 h-6 md:w-8 md:h-8 text-indigo-700">
                                                        <img class="icon icon-tabler icon-tabler-grid"
                                                            src="https://tuk-cdn.s3.amazonaws.com/can-uploader/light-with-button-svg12.svg"
                                                            alt="Produtos" />
                                                    </div>
                                                    <p tabindex="0"
                                                        class="focus:outline-none focus:text-indigo-600 text-indigo-700 xl:text-base md:text-2xl text-base ml-3">
                                                        Produtos</p>
                                                </div>
                                            </div>
                                        </a>
                                    </li>
                                    <li>
                                        <a class="cursor-pointer">
                                            <div class="text-gray-800 pt-8">
                                                <div class="flex items-center justify-between">
                                                    <div class="flex items-center">
                                                        <div class="w-6 h-6 md:w-8 md:h-8 text-gray-800">
                                                            <img class="icon icon-tabler icon-tabler-puzzle"
                                                                src="https://tuk-cdn.s3.amazonaws.com/can-uploader/light-with-button-svg13.svg"
                                                                alt="APIs" />
                                                        </div>
                                                        <p tabindex="0"
                                                            class="focus:outline-none focus:text-indigo-600 text-gray-800 xl:text-base md:text-2xl text-base ml-3">
                                                            APIs</p>
                                                    </div>
                                                </div>
                                            </div>
                                        </a>
                                    </li>
                                    <li>
                                        <a class="cursor-pointer">
                                            <div class="text-gray-800 pt-8">
                                                <div class="flex items-center">
                                                    <div class="w-6 h-6 md:w-8 md:h-8 text-gray-800">
                                                        <img class="icon icon-tabler icon-tabler-compass"
                                                            src="https://tuk-cdn.s3.amazonaws.com/can-uploader/light-with-button-svg14.svg"
                                                            alt="performance" />
                                                    </div>
                                                    <p tabindex="0"
                                                        class="focus:outline-none focus:text-indigo-600 text-gray-800 xl:text-base md:text-2xl text-base ml-3">
                                                        Performance</p>
                                                </div>
                                            </div>
                                        </a>
                                    </li>
                                    <li class="text-gray-800 pt-8 cursor-pointer">
                                        <div class="flex items-center justify-between">
                                            <div class="flex items-center">
                                                <div class="w-6 h-6 md:w-8 md:h-8 text-gray-800">
                                                    <img class="icon icon-tabler icon-tabler-code"
                                                        src="https://tuk-cdn.s3.amazonaws.com/can-uploader/light-with-button-svg15.svg"
                                                        alt="deliverables" />
                                                </div>
                                                <p tabindex="0"
                                                    class="focus:outline-none focus:text-indigo-600 text-gray-800 xl:text-base md:text-2xl text-base ml-3">
                                                    Deliverables</p>
                                            </div>
                                        </div>
                                    </li>
                                </ul>
                            </div>


                            <div class="w-full pt-4">
                                <div class="flex justify-center mb-4 w-full">
                                    <div class="relative w-full">
                                        <div class="text-gray-500 
                                                absolute ml-4 
                                                inset-0 m-auto 
                                                    w-4 h-4">
                                            <img class="icon icon-tabler icon-tabler-search"
                                                src="https://tuk-cdn.s3.amazonaws.com/can-uploader/light-with-button-svg16.svg"
                                                alt="search" />
                                        </div>
                                        <input class="focus:ring-2 
                                            focus:ring-gray-600 bg-gray-100 
                                            focus:outline-none rounded w-full 
                                            text-sm text-gray-500 pl-10 py-2" type="text" placeholder="Search" />
                                    </div>
                                </div>
                                <div class="border-t border-gray-300">
                                    <div class="w-full flex items-center justify-between pt-1">

                                        <ul class="flex">
                                            <li class="cursor-pointer text-gray-800 pt-5 pb-3">
                                                <div tabindex="0"
                                                    class="focus:outline-none focus:text-indigo-600 w-6 h-6 md:w-8 md:h-8">
                                                    <img class="icon icon-tabler icon-tabler-messages"
                                                        src="https://tuk-cdn.s3.amazonaws.com/can-uploader/light-with-button-svg17.svg"
                                                        alt="chat" />
                                                </div>
                                            </li>
                                            <li class="cursor-pointer text-gray-800 pt-5 pb-3 pl-3">
                                                <div tabindex="0"
                                                    class="focus:outline-none focus:text-indigo-600 w-6 h-6 md:w-8 md:h-8">
                                                    <img class="icon icon-tabler icon-tabler-bell"
                                                        src="https://tuk-cdn.s3.amazonaws.com/can-uploader/light-with-button-svg18.svg"
                                                        alt="bell" />
                                                </div>
                                            </li>
                                        </ul>
                                    </div>
                                </div>
                            </div>
                        </div>
                    </div>
                </div>
            </div>
        </nav>

        <script>
            alert("Olá Henrique!")
            function dropdownHandler(element) {
                let single = element.getElementsByTagName("ul")[0];
                single.classList.toggle("hidden");
            }
            function MenuHandler(el, val) {
                let MainList = el.parentElement.parentElement.getElementsByTagName("ul")[0];
                let closeIcon = el.parentElement.parentElement.getElementsByClassName("close-m-menu")[0];
                let showIcon = el.parentElement.parentElement.getElementsByClassName("show-m-menu")[0];
                if (val) {
                    MainList.classList.remove("hidden");
                    el.classList.add("hidden");
                    closeIcon.classList.remove("hidden");
                } else {
                    showIcon.classList.remove("hidden");
                    MainList.classList.add("hidden");
                    el.classList.add("hidden");
                }
            }
            // ------------------------------------------------------
            let sideBar = document.getElementById("mobile-nav");
            let menu = document.getElementById("menu");
            let cross = document.getElementById("cross");
            const sidebarHandler = (check) => {
                if (check) {
                    sideBar.style.transform = "translateX(0px)";
                    menu.classList.add("hidden");
                    cross.classList.remove("hidden");
                } else {
                    sideBar.style.transform = "translateX(-100%)";
                    menu.classList.remove("hidden");
                    cross.classList.add("hidden");
                }
            };
            let list = document.getElementById("list");
            let chevrondown = document.getElementById("chevrondown");
            let chevronup = document.getElementById("chevronup");
            const listHandler = (check) => {
                if (check) {
                    list.classList.remove("hidden");
                    chevrondown.classList.remove("hidden");
                    chevronup.classList.add("hidden");
                } else {
                    list.classList.add("hidden");
                    chevrondown.classList.add("hidden");
                    chevronup.classList.remove("hidden");
                }
            };
            console.log('hello world');
            var log = 3;
            let slides = document.querySelectorAll(".slide-ana>div");
            let slideSayisi = slides.length;
            let prev = document.getElementById("prev");
            let next = document.getElementById("next");
            for (let index = 0; index < slides.length; index++) {
                const element = slides[index];
                element.style.transform = "translateX(" + 100 * index + "%)";
            }
            let loop = 0 + 1000 * slideSayisi;

            function goNext() {
                loop++;
                for (let index = 0; index < slides.length; index++) {
                    const element = slides[index];
                    element.style.transform = "translateX(" + 100 * (index - (loop % slideSayisi)) + "%)";
                }
            }

            function goPrev() {
                loop--;
                for (let index = 0; index < slides.length; index++) {
                    const element = slides[index];
                    element.style.transform = "translateX(" + 100 * (index - (loop % slideSayisi)) + "%)";
                }
            }

            function openView() {
                document.getElementById("viewerButton").classList.add("hidden");
                document.getElementById("viewerBox").classList.remove("hidden");
            }
            function closeView() {
                document.getElementById("viewerBox").classList.add("hidden");
                document.getElementById("viewerButton").classList.remove("hidden");

            }
            function helloDarknessMyOldFriend() {
                {
                    const document.getElementById("viewerBox").C
                }
            }
            console.log("Olá mundo");

        </script>

        <!-- Code block ends -->

        <main class="bg-transparent m-auto">
            <!--m == Margin-->

            <div class="grid grid-cols-1 lg:grid-cols-2">
                <div class="bg-gray-100 dark:bg-transparent py-8 ">
                    <div class="container mx-auto flex flex-col items-center  ">
                        <div class="w-11/12 sm:w-2/3 lg:flex  flex-col   mb-5 sm:mb-10">
                            <h1
                                class="text-2xl sm:text-3xl md:text-4xl lg:text-5xl xl:text-5xl text-initial text-gray-800 font-sans font-black leading-7 md:leading-10">
                                Crie soluções de
                                <span class="text-indigo-700">Fintechs</span>
                                em seu negócio.
                            </h1>
                            <p
                                class="mt-5 sm:mt-10 lg:w-10/12 text-gray-500 font-normal text-initial text-sm sm:text-lg">
                                Uma plataforma profissional de <span class="text-indigo-700">Embedded Finance</span>
                                para que seu negócio ofereça serviços financeiros de acordo com a sua demanda de maneira
                                prática e efetiva.</p>
                        </div>
                        <div class="flex">
                            <button
                                class="focus:outline-none focus:ring-2 focus:ring-offset-2 focus:ring-indigo-700 bg-indigo-700 
                            transition duration-200 ease-in-out hover:bg-indigo-500 lg:text-xl lg:font-bold
                            rounded text-white px-4 sm:px-10 border border-indigo-700 py-2  sm:py-4 text-sm">Iniciar</button>

                        </div>
                    </div>
                </div>
                <!--P8 ==  Padding: 8px;-->
                <div class="lg:min-h-screen lg:flex lg:items-center p-8 sm:p-12">
                    <!--   <div class="flex-grow bg-white shadow-xl rounded-md border border-gray-300 p-8 "> -->
                    <!--<div class="sm:flex sm:items-center">
                            <img src="user.png" alt="Rosto" class="sm: flex-shrink-0 mx-auto sm:mx-0 h-24 rounded-full">
                            <div class="sm:ml-4 sm:text-left text-center">
                                <p class="text-xl">Mariana Silva</p>
                                <p class="text-sm text-gray-600">Gerente de suporte Técnico</p>
                            <div class="mt-4">
                                <button type="button" class="text-red-400 hover:text-white hover:bg-red-400 border border-red-400 font-semibold rounded-md text-xs px-4 py-1 focus:outline-none">HelloWorld</button>
                            </div>
                            </div>
                            
                        </div> -->
                    <!--Formulario-
                        <form class="flex w-full mt-8">
                            <input type="password" placeholder="Sua senha" class="flex-1 w-full text-gray-300 bg-gray-200 rounded-md hover:bg-white border border-gray-200  outline-none focus:bg-white py-2 px-4 ">
                            <button type="button" class="flex-shrink-0 bg-teal-400 hover:bg-teal-600 outline-none py-2 px-4 ml-4 text-white font-semibold rounded-md">
                                Entrar
                            </button>
                        </form> -->
                    <!--</div> -->
                    <img id="homeBanner" class="object-cover max-h-max  " src="template.png" alt="">
                </div>
            </div>
            <!--lg: large, o tamanho que terá em uma tela maior-->

            <div
                class="flex flex-wrap py-4 m-auto items-center space-x-4 sm:grid-cols-1 lg:flex items-center justify-center w-full">
                <h3 class="space-y-6 py-8 text-base leading-7 sm:text-5xl mb-2 lg:text-5xl font-sans pt-10">Ecossistema
                    <span class="text-indigo-700"> Wiress</span> - Tudo em um só lugar
                </h3>
                <p class="text-gray-500 font-sans py-8 px-96 text-2xl">Receba pagamentos, desenvolva novas formas de
                    receita e construa a sua própria
                    experiência de banco digital, de maneira rápida e escalável, conforme sua
                    necessidade. Tudo em uma plataforma única.</p>
            </div>
            <div
                class="flex flex-wrap py-4 m-auto items-center space-x-4 sm:grid-cols-1 lg:flex items-center justify-center w-full">
                <div
                    class="max-w-sm rounded overflow-hidden shadow-lg transition duration-500 ease-in-out transform hover:-translate-y-1 hover:scale-110 ">
                    <div class="px-8 py-4 ">
                        <div class="font-bold text-center text-xl mb-2">
                            <img class="flex items-center px-32" src="icons8-mastercard-64.png" alt="">
                            Emissão de Cartão
                        </div>
                        <p class=" text-base text-center">
                            Emissão de cartão internacional personalizado da bandeira Mastercard.
                        </p>
                    </div>

                </div>
                <div
                    class="max-w-sm rounded overflow-hidden shadow-lg transition duration-500 ease-in-out transform hover:-translate-y-1 hover:scale-110">
                    <div class="px-8 py-4 ">
                        <div class="font-bold text-center text-xl mb-2">
                            <img class="flex items-center px-32" src="wallet.png" alt="">
                            Conta digital
                        </div>
                        <p class=" text-center text-base ">
                            Plataforma White Label para conta digital com a sua marca.
                        </p>
                    </div>
                </div>
                <div
                    class="max-w-sm rounded overflow-hidden shadow-lg transition duration-500 ease-in-out transform hover:-translate-y-1 hover:scale-110">
                    <div class="px-8 py-4 ">
                        <div class="font-bold text-center text-xl mb-2">
                            <img class="flex items-center px-32 " src="pix.png" alt="">
                            Pix Parcelado
                        </div>
                        <p class="text-gray-700 text-center 
                          
                          text-base">
                            Carteira digital de criptomoedas e Staking automático.
                        </p>
                    </div>
                </div>
            </div>
            <div
                class="flex flex-wrap py-4 m-auto items-center space-x-4 sm:grid-cols-1 lg:flex items-center justify-center w-full">
                <div
                    class="max-w-sm rounded overflow-hidden shadow-lg transition duration-500 ease-in-out transform hover:-translate-y-1 hover:scale-110 ">
                    <div class="px-8 py-4">
                        <div class="font-bold text-center text-xl mb-2">
                            <img class="flex items-center px-32" src="lending.png" alt="">
                            Empréstimos
                        </div>
                        <p class="text-gray-700 text-base text-center">
                            Serviços de empréstimos autonomo sem nenhuma instituição financeira.
                        </p>
                    </div>

                </div>
                <div
                    class="max-w-sm rounded overflow-hidden shadow-lg transition duration-500 ease-in-out transform hover:-translate-y-1 hover:scale-110">
                    <div class="px-8 py-4">
                        <div class="font-bold text-center text-xl mb-2">
                            <img class="flex items-center px-32" src="insurance.png" alt="">
                            Seguros
                        </div>
                        <p class="text-gray-700 text-center text-base">
                            Ofereça serviços de seguros sobre seus produtos.
                        </p>
                    </div>
                </div>
                <div
                    class="max-w-sm rounded overflow-hidden shadow-lg transition duration-500 ease-in-out transform hover:-translate-y-1 hover:scale-110">
                    <div class="px-8 py-4">
                        <div class="font-bold text-center text-xl mb-2">
                            <img class="flex items-center px-32" src="statement.png" alt="">
                            Emissão de Boletos
                        </div>
                        <p class="text-gray-700 text-center 
                          
                          text-base">
                            Compra e venda de NFTs para oferecer benefícios e fortalecer sua marca.
                        </p>
                    </div>
                </div>
            </div>
            <!--Division 2.1-->
            <!-- component -->
            <div class="px-3 md:lg:xl:px-40   border-t border-b py-20 bg-opacity-10"
                style="background-image: url('https://www.toptal.com/designers/subtlepatterns/uploads/dot-grid.png') ;">
                <div class="grid grid-cols-1 md:lg:xl:grid-cols-3 group bg-white shadow-xl shadow-neutral-100 border ">


                    <div
                        class="p-10 flex flex-col items-center text-center group md:lg:xl:border-r md:lg:xl:border-b hover:bg-slate-50 cursor-pointer">
                        <span class="p-5 rounded-full bg-red-500 text-white shadow-lg shadow-red-200"><svg
                                xmlns="http://www.w3.org/2000/svg" class="h-10 w-10" fill="none" viewBox="0 0 24 24"
                                stroke="currentColor" stroke-width="1.5">
                                <path stroke-linecap="round" stroke-linejoin="round"
                                    d="M12 4.354a4 4 0 110 5.292M15 21H3v-1a6 6 0 0112 0v1zm0 0h6v-1a6 6 0 00-9-5.197M13 7a4 4 0 11-8 0 4 4 0 018 0z" />
                            </svg></span>
                        <p class="text-xl font-medium text-slate-700 mt-3">Most Experienced Team</p>
                        <p class="mt-2 text-sm text-slate-500">Team BrainEdge education is a bunch of highly focused,
                            energetic
                            set of people.</p>
                    </div>

                    <div
                        class="p-10 flex flex-col items-center text-center group md:lg:xl:border-r md:lg:xl:border-b hover:bg-slate-50 cursor-pointer">
                        <span class="p-5 rounded-full bg-orange-500 text-white shadow-lg shadow-orange-200"><svg
                                xmlns="http://www.w3.org/2000/svg" class="h-10 w-10" fill="none" viewBox="0 0 24 24"
                                stroke="currentColor" stroke-width="1.5">
                                <path d="M14 2H6a2 2 0 0 0-2 2v16a2 2 0 0 0 2 2h12a2 2 0 0 0 2-2V8z"></path>
                                <polyline points="14 2 14 8 20 8"></polyline>
                                <line x1="16" y1="13" x2="8" y2="13"></line>
                                <line x1="16" y1="17" x2="8" y2="17"></line>
                                <polyline points="10 9 9 9 8 9"></polyline>
                            </svg></span>
                        <p class="text-xl font-medium text-slate-700 mt-3">Best
                            Test preparation</p>
                        <p class="mt-2 text-sm text-slate-500">Know where you stand and what next to do to succeed .</p>
                    </div>

                    <div
                        class="p-10 flex flex-col items-center text-center group   md:lg:xl:border-b hover:bg-slate-50 cursor-pointer">
                        <span class="p-5 rounded-full bg-yellow-500 text-white shadow-lg shadow-yellow-200"><svg
                                xmlns="http://www.w3.org/2000/svg" class="h-10 w-10" fill="none" viewBox="0 0 24 24"
                                stroke="currentColor" stroke-width="1.5">
                                <path stroke-linecap="round" stroke-linejoin="round"
                                    d="M17 8h2a2 2 0 012 2v6a2 2 0 01-2 2h-2v4l-4-4H9a1.994 1.994 0 01-1.414-.586m0 0L11 14h4a2 2 0 002-2V6a2 2 0 00-2-2H5a2 2 0 00-2 2v6a2 2 0 002 2h2v4l.586-.586z" />
                            </svg></span>
                        <p class="text-xl font-medium text-slate-700 mt-3">Admission process Guidance</p>
                        <p class="mt-2 text-sm text-slate-500">Professional Advice for higher education abroad and
                            select the
                            top institutions worldwide.</p>
                    </div>


                    <div
                        class="p-10 flex flex-col items-center text-center group   md:lg:xl:border-r hover:bg-slate-50 cursor-pointer">
                        <span class="p-5 rounded-full bg-lime-500 text-white shadow-lg shadow-lime-200"><svg
                                xmlns="http://www.w3.org/2000/svg" class="h-10 w-10" fill="none" viewBox="0 0 24 24"
                                stroke="currentColor" stroke-width="1.5">
                                <path stroke-linecap="round" stroke-linejoin="round"
                                    d="M13 7h8m0 0v8m0-8l-8 8-4-4-6 6" />
                            </svg></span>
                        <p class="text-xl font-medium text-slate-700 mt-3">Best
                            Track Record</p>
                        <p class="mt-2 text-sm text-slate-500">Yet another year ! Yet another jewel in our crown!</p>
                    </div>

                    <div
                        class="p-10 flex flex-col items-center text-center group    md:lg:xl:border-r hover:bg-slate-50 cursor-pointer">
                        <span class="p-5 rounded-full bg-teal-500 text-white shadow-lg shadow-teal-200"><svg
                                xmlns="http://www.w3.org/2000/svg" class="h-10 w-10" fill="none" viewBox="0 0 24 24"
                                stroke="currentColor" stroke-width="1.5">
                                <path stroke-linecap="round" stroke-linejoin="round"
                                    d="M9 5H7a2 2 0 00-2 2v12a2 2 0 002 2h10a2 2 0 002-2V7a2 2 0 00-2-2h-2M9 5a2 2 0 002 2h2a2 2 0 002-2M9 5a2 2 0 012-2h2a2 2 0 012 2m-3 7h3m-3 4h3m-6-4h.01M9 16h.01" />
                            </svg></span>
                        <p class="text-xl font-medium text-slate-700 mt-3">Free
                            Mock Exams</p>
                        <p class="mt-2 text-sm text-slate-500">Get Topic-Wise Tests, Section- Wise and mock tests for
                            your
                            preparation.</p>
                    </div>

                    <div class="bg-white  rounded-lg px-6 py-8 ring-1 ring-slate-900/5 shadow-xl">
                        <div>
                          <span class="inline-flex items-center justify-center p-2 bg-indigo-500 rounded-md shadow-lg">
                            <svg
                                xmlns="http://www.w3.org/2000/svg" class="h-10 w-10" fill="none" viewBox="0 0 24 24"
                                stroke="currentColor" stroke-width="1.5">
                                <path stroke-linecap="round" stroke-linejoin="round"
                                    d="M9 5H7a2 2 0 00-2 2v12a2 2 0 002 2h10a2 2 0 002-2V7a2 2 0 00-2-2h-2M9 5a2 2 0 002 2h2a2 2 0 002-2M9 5a2 2 0 012-2h2a2 2 0 012 2m-3 7h3m-3 4h3m-6-4h.01M9 16h.01" />
                            </svg>
                          </span>
                        </div>
                        <h3 class="text-slate-900  mt-5 text-base font-medium tracking-tight">Writes Upside-Down</h3>
                        <p class="text-slate-500  mt-2 text-sm">
                          The Zero Gravity Pen can be used to write in any orientation, including upside-down. It even works in outer space.
                        </p>
                      </div>




                </div>

                <div
                    class="w-full   bg-indigo-600 shadow-xl shadow-indigo-200 py-10 px-20 flex justify-between items-center">
                    <p class=" text-white"> <span class="text-4xl font-medium">Still Confused ?</span> <br> <span
                            class="text-lg">Book For Free Career Consultation Today ! </span></p>
                    <button
                        class="px-5 py-3  font-medium text-slate-700 shadow-xl  hover:bg-white duration-150  bg-yellow-400">BOOK
                        AN APPOINTMENT </button>
                </div>

            </div>

            <!--Cards-->
            <!-- component -->
            <div class="relative flex min-h-screen flex-col justify-center overflow-hidden bg-gray-50 py-6 sm:py-12">
                <img src="/img/beams.jpg" alt=""
                    class="absolute top-1/2 left-1/2 max-w-none -translate-x-1/2 -translate-y-1/2" width="1308" />
                <div
                    class="absolute inset-0 bg-[url(/img/grid.svg)] bg-center [mask-image:linear-gradient(180deg,white,rgba(255,255,255,0))]">
                </div>
                <div class="flex flex-col hidden md:block -space-y-72 items-center relative">

                    <div
                        class="relative shadow-2xl shadow-[#16192E] z-30 bg-transparent stroke-1 -rotate-[60deg] skew-y-[30deg] scale-75 border-gray-200 w-[650px] mx-auto h-[420px] rounded-3xl">
                        <div
                            class="w-full h-full absolute top-0 left-0 rounded-3xl bg-cover bg-[url('https://products.ls.graphics/mesh-gradients/images/37.-Light-Sky-Blue_1.jpg')]">
                            <div class="p-12 flex flex-col justify-between h-full">
                                <img class="h-24 w-24"
                                    src="https://upload.wikimedia.org/wikipedia/commons/5/5e/Visa_Inc._logo.svg" alt="">
                                <div class="flex flex-col">
                                    <p class="text-gray-500 text-lg font-mono">1253 8282 2588 23562</p>
                                    <p class="font-bold text-lg text-stone-600">Robert</p>
                                </div>
                            </div>
                        </div>
                    </div>
                    <div
                        class="relative shadow-2xl shadow-[#16192E] z-20 bg-transparent stroke-1 -rotate-[60deg] skew-y-[30deg] scale-75 border-gray-200 w-[650px] mx-auto h-[420px] rounded-3xl">
                        <div
                            class="w-full h-full absolute top-0 left-0 rounded-3xl bg-cover bg-[url('https://products.ls.graphics/mesh-gradients/images/35.-Ronchi.jpg')]">
                            <div class="p-12 flex flex-col justify-between h-full">
                                <img class="h-28 w-28"
                                    src="https://upload.wikimedia.org/wikipedia/commons/5/57/Discover_Card_logo.svg"
                                    alt="">
                                <div class="flex flex-col">
                                    <p class="text-gray-300 text-lg font-mono">1253 8282 2588 23562</p>
                                    <p class="font-bold text-lg text-stone-300">Caroline Q.</p>
                                </div>
                            </div>
                        </div>
                    </div>
                    <div
                        class="relative shadow-2xl shadow-[#16192E] z-10 bg-transparent stroke-1  -rotate-[60deg] skew-y-[30deg] scale-75 w-[650px] mx-auto h-[420px] rounded-3xl">
                        <div
                            class="w-full h-full absolute top-0 left-0 rounded-3xl bg-cover bg-[url('https://products.ls.graphics/mesh-gradients/images/15.-Perfume_1.jpg')]">
                            <div class="p-12 flex flex-col justify-between h-full">
                                <img class="h-24 w-24"
                                    src="https://upload.wikimedia.org/wikipedia/commons/5/5e/Visa_Inc._logo.svg" alt="">
                                <div class="flex flex-col">
                                    <p class="text-gray-500 text-lg font-mono">1253 8282 2588 23562</p>
                                    <p class="font-bold text-lg text-stone-600">Robert Lewonsky</p>
                                </div>
                            </div>
                        </div>
                    </div>
                </div>
            </div>
            <!--End Cardss-->
            
            <!--End Division 2.1-->
            <!--Division #3-->
            <div class="2xl:container 2xl:mx-auto md:py-12 lg:px-20 md:px-6 py-9 px-4">
                <div id="viewerButton" class="hidden w-full flex justify-center">
                    <button onclick="openView()"
                        class="bg-white text-indigo-600 shadow-md rounded focus:outline-none focus:ring-2 focus:ring-offset-2 focus:ring-indigo-600 py-5 px-10 font-semibold">Open
                        Quick View</button>
                </div>
                <div id="viewerBox" class="lg:p-10 md:p-6 p-4 bg-white">
                    <div class="flex justify-end">
                        <button onclick="closeView()" aria-label="Close"
                            class="focus:outline-none focus:ring-2 focus:ring-gray-800">
                            <img class="dark:hidden"
                                src="https://tuk-cdn.s3.amazonaws.com/can-uploader/quick-view-2-svg1.svg" alt="cross">
                            <img class="dark:block hidden"
                                src="https://tuk-cdn.s3.amazonaws.com/can-uploader/quick-view-2-svg1dark.svg"
                                alt="cross">
                        </button>
                    </div>
                    <!--
                    <div class="mt-3 md:mt-4 lg:mt-0 flex flex-col lg:flex-row items-strech justify-center lg:space-x-8">
                        <div class="lg:w-1/2 flex justify-between items-strech bg-gray-50  px-2 py-20 md:py-6 md:px-6 lg:py-24">
                            <div class="flex items-center">
                                <button onclick="goPrev()" aria-label="slide back" class="focus:outline-none focus:ring-2 focus:ring-gray-800 hover:bg-gray-100">
                                    <img class="" src="https://tuk-cdn.s3.amazonaws.com/can-uploader/quick-view-2-svg2.svg" alt="previous">
                                </button>
                            </div>
                            <div class="slider">
                                <div class="slide-ana lg:relative">
                                    <div class="flex" style="transform: translateX(-100%)">
                                        <img src="https://i.ibb.co/fMGD6ZC/eugene-chystiakov-3ne-Swyntb-Q8-unsplash-1-removebg-preview-3-1.png" alt="A black chair with wooden legs" class="w-full h-full" />
                                    </div>
                                    <div class="flex" style="transform: translateX(0%)">
                                        <img src="https://i.ibb.co/fMGD6ZC/eugene-chystiakov-3ne-Swyntb-Q8-unsplash-1-removebg-preview-3-1.png" alt="A black chair with wooden legs" class="w-full h-full" />
                                    </div>
                                    <div class="flex" style="transform: translateX(100%)">
                                        <img src="https://i.ibb.co/fMGD6ZC/eugene-chystiakov-3ne-Swyntb-Q8-unsplash-1-removebg-preview-3-1.png" alt="A black chair with wooden legs" class="w-full h-full" />
                                    </div>
                                </div>
                            </div>
                            <div class="flex items-center">
                                <button onclick="goNext()" aria-label="slide forward" class="focus:outline-none focus:ring-2 focus:ring-gray-800 hover:bg-gray-100">
                                    <img class="transform -rotate-180" src="https://tuk-cdn.s3.amazonaws.com/can-uploader/quick-view-2-svg2.svg" alt="next">
                                </button>
                            </div>
                        </div> -->
                    <div
                        class="mt-3 md:mt-4 lg:mt-0 flex flex-col lg:flex-row items-strech justify-center lg:space-x-8">
                        <div class="lg:w-1/2 flex justify-between items-strech  md:py-6 md:px-6 lg:py-20">

                            <div class="">
                                <img class="object-cover h-full w-full" src="code.png" alt="">

                            </div>

                        </div>
                        <div class="lg:w-1/2 flex flex-col -mt-7  -py-8 md:mt-8 lg:mt-0 pb-2 lg:pb-0">
                            <h1 class="text-2xl lg:text-4xl font-semibold text-gray-800 py-8">Integre a API da Wiress no
                                seu sistema com:</h1>
                            <ul class="space-y-4">
                                <li class="flex items-center">
                                    <svg class="h-6 w-6 flex-none fill-sky-100 stroke-sky-500 stroke-2"
                                        stroke-linecap="round" stroke-linejoin="round">
                                        <circle cx="12" cy="12" r="11" />
                                        <path d="m8 13 2.165 2.165a1 1 0 0 0 1.521-.126L16 9" fill="none" />
                                    </svg>
                                    <p class="ml-4">
                                        Segurança
                                    </p>
                                </li>
                                <li class="flex items-center">
                                    <svg class="h-6 w-6 flex-none fill-sky-100 stroke-sky-500 stroke-2"
                                        stroke-linecap="round" stroke-linejoin="round">
                                        <circle cx="12" cy="12" r="11" />
                                        <path d="m8 13 2.165 2.165a1 1 0 0 0 1.521-.126L16 9" fill="none" />
                                    </svg>
                                    <p class="ml-4">
                                        Disbonibilidade de garantia
                                    </p>
                                </li>
                                <li class="flex items-center">
                                    <svg class="h-6 w-6 flex-none fill-sky-100 stroke-sky-500 stroke-2"
                                        stroke-linecap="round" stroke-linejoin="round">
                                        <circle cx="12" cy="12" r="11" />
                                        <path d="m8 13 2.165 2.165a1 1 0 0 0 1.521-.126L16 9" fill="none" />
                                    </svg>
                                    <p class="ml-4">Criptografia de ponta a ponta</p>
                                </li>
                                <li class="flex items-center">
                                    <svg class="h-6 w-6 flex-none fill-sky-100 stroke-sky-500 stroke-2"
                                        stroke-linecap="round" stroke-linejoin="round">
                                        <circle cx="12" cy="12" r="11" />
                                        <path d="m8 13 2.165 2.165a1 1 0 0 0 1.521-.126L16 9" fill="none" />
                                    </svg>
                                    <p class="ml-4">Agilidade</p>
                                </li>
                                <li class="flex items-center">
                                    <svg class="h-6 w-6 flex-none fill-sky-100 stroke-sky-500 stroke-2"
                                        stroke-linecap="round" stroke-linejoin="round">
                                        <circle cx="12" cy="12" r="11" />
                                        <path d="m8 13 2.165 2.165a1 1 0 0 0 1.521-.126L16 9" fill="none" />
                                    </svg>
                                    <p class="ml-4">Suporte Técnico</p>
                                </li>

                            </ul>
                            <div
                                class="flex items-center flex-col md:flex-row space-y-4 md:space-y-0 md:space-x-6 lg:space-x-8 md:mt-16 py-2">
                                <button
                                    class="w-full md:w-3/5 border border-gray-800 text-base font-medium leading-none text-white uppercase py-6 focus:outline-none focus:ring-2 focus:ring-offset-2 focus:ring-gray-800 bg-gray-800 text-white dark:bg-white dark:text-gray-900 dark:hover:bg-gray-200">Add
                                    to Cart</button>
                                <button
                                    class="w-full md:w-2/5 border border-gray-800 text-base font-medium leading-none text-gray-800 uppercase py-6 bg-transparent focus:outline-none focus:ring-2 focus:ring-offset-2   focus:ring-gray-800 hover:bg-gray-800 hover:text-white  ">View
                                    Details</button>
                            </div>
                        </div>
                    </div>
                </div>
            </div>
            <!--End Division #3-->

            <!--Division #4-->
            <!--Cards-->
            <div class="flex flex wrap flex items-center sm:grid-cols-1 lg:flex items-center justify-center w-full">
                <div
                    class="max-w-sm bg-white rounded-lg border border-gray-200 shadow-md dark:bg-gray-800 dark:border-gray-700 flex items-center">
                    <a href="#">
                        <img class="rounded-t-lg" src="/docs/images/blog/image-1.jpg" alt="" />
                    </a>
                    <div class="p-5">
                        <a href="#">
                            <h5 class="mb-2 text-2xl font-bold tracking-tight text-gray-900 dark:text-white">Noteworthy
                                technology acquisitions 2021</h5>
                        </a>
                        <p class="mb-3 font-normal text-gray-700 dark:text-gray-400">Here are the biggest enterprise
                            technology acquisitions of 2021 so far, in reverse chronological order.</p>
                        <a href="#"
                            class="inline-flex items-center py-2 px-3 text-sm font-medium text-center text-white bg-blue-700 rounded-lg hover:bg-blue-800 focus:ring-4 focus:outline-none focus:ring-blue-300 dark:bg-blue-600 dark:hover:bg-blue-700 dark:focus:ring-blue-800">
                            Read more
                            <svg class="ml-2 -mr-1 w-4 h-4" fill="currentColor" viewBox="0 0 20 20"
                                xmlns="http://www.w3.org/2000/svg">
                                <path fill-rule="evenodd"
                                    d="M10.293 3.293a1 1 0 011.414 0l6 6a1 1 0 010 1.414l-6 6a1 1 0 01-1.414-1.414L14.586 11H3a1 1 0 110-2h11.586l-4.293-4.293a1 1 0 010-1.414z"
                                    clip-rule="evenodd"></path>
                            </svg>
                        </a>
                    </div>
                </div>
                <div
                    class="max-w-sm bg-white rounded-lg border border-gray-200 shadow-md dark:bg-gray-800 dark:border-gray-700 flex items-center">
                    <a href="#">
                        <img class="rounded-t-lg" src="/docs/images/blog/image-1.jpg" alt="" />
                    </a>
                    <div class="p-5">
                        <a href="#">
                            <h5 class="mb-2 text-2xl font-bold tracking-tight text-gray-900 dark:text-white">Noteworthy
                                technology acquisitions 2021</h5>
                        </a>
                        <p class="mb-3 font-normal text-gray-700 dark:text-gray-400">Here are the biggest enterprise
                            technology acquisitions of 2021 so far, in reverse chronological order.</p>
                        <a href="#"
                            class="inline-flex items-center py-2 px-3 text-sm font-medium text-center text-white bg-blue-700 rounded-lg hover:bg-blue-800 focus:ring-4 focus:outline-none focus:ring-blue-300 dark:bg-blue-600 dark:hover:bg-blue-700 dark:focus:ring-blue-800">
                            Read more
                            <svg class="ml-2 -mr-1 w-4 h-4" fill="currentColor" viewBox="0 0 20 20"
                                xmlns="http://www.w3.org/2000/svg">
                                <path fill-rule="evenodd"
                                    d="M10.293 3.293a1 1 0 011.414 0l6 6a1 1 0 010 1.414l-6 6a1 1 0 01-1.414-1.414L14.586 11H3a1 1 0 110-2h11.586l-4.293-4.293a1 1 0 010-1.414z"
                                    clip-rule="evenodd"></path>
                            </svg>
                        </a>
                    </div>
                </div>
                <div
                    class="max-w-sm bg-white rounded-lg border border-gray-200 shadow-md dark:bg-gray-800 dark:border-gray-700 flex items-center">
                    <a href="#">
                        <img class="rounded-t-lg" src="/docs/images/blog/image-1.jpg" alt="" />
                    </a>
                    <div class="p-5">
                        <a href="#">
                            <h5 class="mb-2 text-2xl font-bold tracking-tight text-gray-900 dark:text-white">Noteworthy
                                technology acquisitions 2021</h5>
                        </a>
                        <p class="mb-3 font-normal text-gray-700 dark:text-gray-400">Here are the biggest enterprise
                            technology acquisitions of 2021 so far, in reverse chronological order.</p>
                        <a href="#"
                            class="inline-flex items-center py-2 px-3 text-sm font-medium text-center text-white bg-blue-700 rounded-lg hover:bg-blue-800 focus:ring-4 focus:outline-none focus:ring-blue-300 dark:bg-blue-600 dark:hover:bg-blue-700 dark:focus:ring-blue-800">
                            Read more
                            <svg class="ml-2 -mr-1 w-4 h-4" fill="currentColor" viewBox="0 0 20 20"
                                xmlns="http://www.w3.org/2000/svg">
                                <path fill-rule="evenodd"
                                    d="M10.293 3.293a1 1 0 011.414 0l6 6a1 1 0 010 1.414l-6 6a1 1 0 01-1.414-1.414L14.586 11H3a1 1 0 110-2h11.586l-4.293-4.293a1 1 0 010-1.414z"
                                    clip-rule="evenodd"></path>
                            </svg>
                        </a>
                    </div>
                </div>
            </div>
            <!--End Division #4-->

            <!--Division #5-->
            <div class="px-6 pb-6">
                <dh-component>
                    <div
                        class="container mx-auto grid sm:grid-cols-1 md:grid-cols-2 lg:grid-cols-3 xl:grid-cols-3 pt-6 gap-8">
                        <!-- Remove class [ h-24 ] when adding a card block -->
                        <!-- Remove class [ border-gray-300  dark:border-gray-700 border-dashed border-2 ] to remove dotted border -->
                        <div class="rounded border-gray-300 dark:border-gray-700 border-dashed border-2 h-24 w-12">
                        </div>
                        <!-- Remove class [ h-24 ] when adding a card block -->
                        <!-- Remove class [ border-gray-300  dark:border-gray-700 border-dashed border-2 ] to remove dotted border -->
                        <div class="rounded border-gray-300 dark:border-gray-700 border-dashed border-2 h-24 w-96">
                        </div>
                        <!-- Remove class [ h-24 ] when adding a card block -->
                        <!-- Remove class [ border-gray-300  dark:border-gray-700 border-dashed border-2 ] to remove dotted border -->
                        <div class="rounded border-gray-300 dark:border-gray-700 border-dashed border-2 h-24 w-12">
                        </div>
                    </div>
                </dh-component>
            </div>
        </main>

        <footer>
            <div class="mx-auto container py-16 xl:px-20 lg:px-12 sm:px-6 px-4">
                <div class="grid grid-cols-2 md:grid-cols-3 lg:grid-cols-3 xl:grid-cols-4 md:gap-8 gap-4">
                    <div class="flex flex-col flex-shrink-0">
                        <div class="">
                            <h2 class="hidden sm:block text-base text-xl text-gray-700 font-bold leading-normal px">
                                Wiress</h2>

                        </div>
                        <p class="text-sm leading-none text-gray-800 mt-4 ">Copyright © 2021 Wiress</p>
                        <p class="text-sm leading-none text-gray-800 mt-4 ">All rights reserved</p>
                        <div class="flex items-center gap-x-4 mt-12">
                            <button aria-label="instagram"
                                class="focus:outline-none focus:ring-2 focus:ring-offset-2 focus:ring-gray-800 opacity-50 w-8 h-8 flex-shrink-0 bg-gray-800 cursor-pointer hover:bg-gray-700 rounded-full flex items-center justify-center">
                                <svg width="18" height="17" viewBox="0 0 18 17" fill="none"
                                    xmlns="http://www.w3.org/2000/svg">
                                    <path fill-rule="evenodd" clip-rule="evenodd"
                                        d="M9.00081 0.233398C6.68327 0.233398 6.39243 0.243215 5.48219 0.283343C4.57374 0.323644 3.95364 0.462973 3.41106 0.667403C2.84981 0.87855 2.37372 1.161 1.8994 1.62066C1.42473 2.08016 1.13317 2.54137 0.914502 3.08491C0.702944 3.61071 0.558942 4.2116 0.518053 5.09132C0.477342 5.97311 0.466675 6.25504 0.466675 8.50015C0.466675 10.7453 0.476986 11.0262 0.518231 11.9079C0.560009 12.788 0.703833 13.3887 0.914679 13.9144C1.13282 14.4581 1.42437 14.9193 1.89887 15.3788C2.37301 15.8386 2.8491 16.1218 3.40999 16.3329C3.95293 16.5373 4.57321 16.6767 5.48148 16.717C6.39171 16.7571 6.68238 16.7669 8.99974 16.7669C11.3175 16.7669 11.6074 16.7571 12.5176 16.717C13.4261 16.6767 14.0469 16.5373 14.5898 16.3329C15.1509 16.1218 15.6263 15.8386 16.1004 15.3788C16.5751 14.9193 16.8667 14.4581 17.0853 13.9145C17.2951 13.3887 17.4391 12.7878 17.4818 11.9081C17.5227 11.0263 17.5333 10.7453 17.5333 8.50015C17.5333 6.25504 17.5227 5.97328 17.4818 5.09149C17.4391 4.21143 17.2951 3.61071 17.0853 3.08508C16.8667 2.54137 16.5751 2.08016 16.1004 1.62066C15.6258 1.16082 15.1511 0.878377 14.5893 0.667403C14.0453 0.462973 13.4249 0.323644 12.5164 0.283343C11.6062 0.243215 11.3164 0.233398 8.99814 0.233398H9.00081ZM8.23525 1.72311C8.46245 1.72277 8.71597 1.72311 9.00077 1.72311C11.2792 1.72311 11.5492 1.73104 12.449 1.77065C13.281 1.8075 13.7326 1.94218 14.0334 2.05533C14.4316 2.20517 14.7155 2.38428 15.014 2.67362C15.3127 2.96295 15.4976 3.23851 15.6526 3.62429C15.7694 3.91535 15.9086 4.3528 15.9464 5.15881C15.9873 6.03026 15.9962 6.29204 15.9962 8.49823C15.9962 10.7044 15.9873 10.9662 15.9464 11.8377C15.9084 12.6437 15.7694 13.0811 15.6526 13.3722C15.4979 13.758 15.3127 14.0327 15.014 14.3218C14.7153 14.6112 14.4318 14.7903 14.0334 14.9401C13.7329 15.0538 13.281 15.1881 12.449 15.225C11.5494 15.2646 11.2792 15.2732 9.00077 15.2732C6.72217 15.2732 6.45212 15.2646 5.55256 15.225C4.72055 15.1878 4.26899 15.0531 3.96801 14.9399C3.56978 14.7901 3.28533 14.611 2.98666 14.3216C2.68799 14.0323 2.5031 13.7574 2.34808 13.3715C2.23128 13.0804 2.09208 12.643 2.05421 11.837C2.01332 10.9655 2.00514 10.7037 2.00514 8.49617C2.00514 6.2886 2.01332 6.0282 2.05421 5.15674C2.09226 4.35073 2.23128 3.91329 2.34808 3.62188C2.50275 3.2361 2.68799 2.96054 2.98666 2.67121C3.28533 2.38187 3.56978 2.20276 3.96801 2.05258C4.26881 1.93891 4.72055 1.80457 5.55256 1.76755C6.33977 1.7331 6.64484 1.72277 8.23525 1.72105V1.72311ZM13.5558 3.09574C12.9905 3.09574 12.5318 3.53956 12.5318 4.08741C12.5318 4.63508 12.9905 5.07942 13.5558 5.07942C14.1212 5.07942 14.5799 4.63508 14.5799 4.08741C14.5799 3.53974 14.1212 3.09574 13.5558 3.09574ZM9.00082 4.25481C6.58071 4.25481 4.61855 6.15564 4.61855 8.50013C4.61855 10.8446 6.58071 12.7446 9.00082 12.7446C11.4209 12.7446 13.3824 10.8446 13.3824 8.50013C13.3824 6.15564 11.4209 4.25481 9.00082 4.25481ZM9.00079 5.74454C10.5717 5.74454 11.8453 6.97818 11.8453 8.50013C11.8453 10.0219 10.5717 11.2557 9.00079 11.2557C7.42975 11.2557 6.15632 10.0219 6.15632 8.50013C6.15632 6.97818 7.42975 5.74454 9.00079 5.74454Z"
                                        fill="white" />
                                </svg>
                            </button>
                            <button aria-label="linked-in"
                                class="focus:outline-none focus:ring-2 focus:ring-offset-2 focus:ring-gray-800 opacity-50 w-8 h-8 flex-shrink-0 bg-gray-800 cursor-pointer hover:bg-gray-700 rounded-full flex items-center justify-center">
                                <svg width="18" height="17" viewBox="0 0 18 17" fill="none"
                                    xmlns="http://www.w3.org/2000/svg">
                                    <path fill-rule="evenodd" clip-rule="evenodd"
                                        d="M17.5333 8.4886C17.5333 9.04766 17.4746 9.60594 17.3592 10.1501C17.2467 10.6814 17.08 11.203 16.8617 11.7016C16.6483 12.1914 16.3837 12.6634 16.0745 13.1035C15.77 13.5409 15.4191 13.9512 15.0337 14.3253C14.6474 14.6977 14.2224 15.0367 13.7711 15.333C13.3152 15.6304 12.8273 15.8864 12.3215 16.094C11.806 16.3044 11.2664 16.4657 10.7184 16.5745C10.1559 16.6866 9.57755 16.7438 8.99962 16.7438C8.42126 16.7438 7.8429 16.6866 7.28121 16.5745C6.73244 16.4657 6.19283 16.3044 5.67779 16.094C5.17195 15.8864 4.68357 15.6304 4.22772 15.333C3.77645 15.0367 3.35143 14.6977 2.96599 14.3253C2.58015 13.9512 2.22928 13.5409 1.92427 13.1035C1.61675 12.6634 1.35172 12.1913 1.13755 11.7016C0.919183 11.203 0.752114 10.6814 0.639188 10.1501C0.525025 9.60594 0.466675 9.04766 0.466675 8.4886C0.466675 7.92913 0.524992 7.36965 0.639221 6.82665C0.752147 6.29538 0.919216 5.77299 1.13759 5.27519C1.35175 4.78505 1.61678 4.31265 1.9243 3.87246C2.22931 3.43473 2.58018 3.02517 2.96602 2.65069C3.35146 2.27823 3.77648 1.94007 4.22775 1.64421C4.6836 1.3455 5.17198 1.08958 5.67783 0.881567C6.19286 0.670713 6.73244 0.509099 7.28124 0.401087C7.84294 0.289844 8.4213 0.233398 8.99966 0.233398C9.57758 0.233398 10.1559 0.289844 10.7185 0.401087C11.2664 0.509131 11.806 0.670745 12.3215 0.881567C12.8273 1.08955 13.3153 1.3455 13.7711 1.64421C14.2224 1.94007 14.6475 2.27823 15.0337 2.65069C15.4191 3.02517 15.77 3.43473 16.0746 3.87246C16.3837 4.31265 16.6483 4.78508 16.8617 5.27519C17.08 5.77299 17.2467 6.29538 17.3592 6.82665C17.4746 7.36965 17.5333 7.92913 17.5333 8.4886ZM5.89026 2.11217C3.85805 3.0405 2.34131 4.85195 1.86836 7.03507C2.06048 7.03668 5.0973 7.07377 8.59622 6.17446C7.33492 4.00666 5.98735 2.23757 5.89026 2.11217ZM9.2 7.26001C5.44774 8.34669 1.84711 8.2685 1.71795 8.26369C1.71585 8.33945 1.71211 8.4128 1.71211 8.4886C1.71211 10.2996 2.41839 11.9507 3.57929 13.1991C3.57678 13.1954 5.57108 9.77282 9.50377 8.54262C9.59876 8.51199 9.69546 8.48456 9.79128 8.45797C9.60838 8.05732 9.40875 7.65584 9.2 7.26001ZM13.8124 3.1977C12.5293 2.10329 10.8447 1.43946 8.9996 1.43946C8.40748 1.43946 7.83286 1.50879 7.28242 1.63697C7.39157 1.77887 8.76042 3.53549 10.0067 5.74921C12.7565 4.75199 13.7944 3.22348 13.8124 3.1977ZM10.288 9.6261C10.2718 9.63131 10.2556 9.6358 10.2397 9.64142C5.93997 11.0914 4.53583 14.0136 4.52064 14.0455C5.75781 14.9762 7.30956 15.5377 8.99965 15.5377C10.0088 15.5377 10.9701 15.339 11.8448 14.9791C11.7368 14.3632 11.3135 12.2042 10.288 9.6261ZM13.0719 14.3349C14.7082 13.2668 15.8703 11.5706 16.1945 9.60591C16.0445 9.55916 14.0057 8.93477 11.6535 9.29958C12.6093 11.8407 12.9977 13.9101 13.0719 14.3349ZM10.5676 6.79966C10.7368 7.13585 10.9006 7.47801 11.0518 7.82188C11.1056 7.94524 11.1581 8.06618 11.2093 8.18708C13.7128 7.88233 16.1792 8.39506 16.2846 8.41599C16.2679 6.74483 15.65 5.21108 14.6275 4.01032C14.6137 4.02922 13.4449 5.66294 10.5676 6.79966Z"
                                        fill="white" />
                                </svg>
                            </button>
                            <button aria-label="twitter"
                                class="focus:outline-none focus:ring-2 focus:ring-offset-2 focus:ring-gray-800 opacity-50 w-8 h-8 flex-shrink-0 bg-gray-800 cursor-pointer hover:bg-gray-700 rounded-full flex items-center justify-center">
                                <svg width="16" height="13" viewBox="0 0 16 13" fill="none"
                                    xmlns="http://www.w3.org/2000/svg">
                                    <path fill-rule="evenodd" clip-rule="evenodd"
                                        d="M7.5208 3.59864L7.55438 4.13498L6.99479 4.0693C4.95791 3.81755 3.17843 2.9638 1.66756 1.52992L0.928908 0.818458L0.73865 1.34385C0.33575 2.51503 0.593158 3.75188 1.43253 4.58375C1.8802 5.04346 1.77948 5.10914 1.00725 4.8355C0.73865 4.74793 0.503625 4.68226 0.481242 4.71509C0.4029 4.79171 0.6715 5.78776 0.884142 6.18181C1.17513 6.72909 1.76828 7.26542 2.4174 7.58284L2.96579 7.83459L2.31668 7.84554C1.68994 7.84554 1.66756 7.85648 1.73471 8.08634C1.95854 8.79781 2.84268 9.55305 3.82755 9.88142L4.52143 10.1113L3.91708 10.4615C3.02175 10.965 1.96973 11.2496 0.917717 11.2715C0.414092 11.2825 0 11.3262 0 11.3591C0 11.4685 1.36538 12.0815 2.15999 12.3223C4.54382 13.0338 7.37531 12.7273 9.50173 11.5123C11.0126 10.6476 12.5235 8.92915 13.2286 7.26542C13.6091 6.37883 13.9896 4.75888 13.9896 3.98174C13.9896 3.47824 14.0232 3.41257 14.6499 2.81056C15.0192 2.4603 15.3662 2.0772 15.4333 1.96775C15.5452 1.75978 15.534 1.75978 14.9633 1.94586C14.012 2.27422 13.8777 2.23044 14.3477 1.73789C14.6947 1.38763 15.1088 0.752784 15.1088 0.566709C15.1088 0.533872 14.9409 0.5886 14.7506 0.68711C14.5492 0.796566 14.1015 0.96075 13.7658 1.05926L13.1614 1.24534L12.613 0.884131C12.3108 0.68711 11.8856 0.468198 11.6617 0.402524C11.0909 0.249286 10.218 0.271177 9.70318 0.446307C8.30422 0.938859 7.42008 2.20855 7.5208 3.59864Z"
                                        fill="white" />
                                </svg>
                            </button>
                            <button aria-label="youtube"
                                class="focus:outline-none focus:ring-2 focus:ring-offset-2 focus:ring-gray-800 opacity-50 w-8 h-8 flex-shrink-0 bg-gray-800 cursor-pointer hover:bg-gray-700 rounded-full flex items-center justify-center">
                                <svg width="18" height="13" viewBox="0 0 18 13" fill="none"
                                    xmlns="http://www.w3.org/2000/svg">
                                    <path fill-rule="evenodd" clip-rule="evenodd"
                                        d="M15.6677 1.17143C16.4021 1.36664 16.9804 1.94183 17.1767 2.67227C17.5333 3.99611 17.5333 6.75832 17.5333 6.75832C17.5333 6.75832 17.5333 9.52043 17.1767 10.8444C16.9804 11.5748 16.4021 12.15 15.6677 12.3453C14.3369 12.7 9.00001 12.7 9.00001 12.7C9.00001 12.7 3.66309 12.7 2.33218 12.3453C1.59783 12.15 1.0195 11.5748 0.823232 10.8444C0.466675 9.52043 0.466675 6.75832 0.466675 6.75832C0.466675 6.75832 0.466675 3.99611 0.823232 2.67227C1.0195 1.94183 1.59783 1.36664 2.33218 1.17143C3.66309 0.81665 9.00001 0.81665 9.00001 0.81665C9.00001 0.81665 14.3369 0.81665 15.6677 1.17143ZM7.40002 4.43326V9.59993L11.6667 7.01669L7.40002 4.43326Z"
                                        fill="white" />
                                </svg>
                            </button>
                        </div>
                    </div>
                    <div class="sm:ml-0 ml-8 flex flex-col">
                        <h2 class="text-base font-semibold leading-4 text-gray-800 ">Company</h2>
                        <a href="javascript:void(0)"
                            class="focus:outline-none focus:underline hover:text-gray-500 text-base leading-4 mt-6 text-gray-800  cursor-pointer">Blog</a>
                        <a href="javascript:void(0)"
                            class="focus:outline-none focus:underline hover:text-gray-500 text-base leading-4 mt-6 text-gray-800  cursor-pointer">Pricing</a>
                        <a href="javascript:void(0)"
                            class="focus:outline-none focus:underline hover:text-gray-500 text-base leading-4 mt-6 text-gray-800  cursor-pointer">About
                            Us</a>
                        <a href="javascript:void(0)"
                            class="focus:outline-none focus:underline hover:text-gray-500 text-base leading-4 mt-6 text-gray-800  cursor-pointer">Contact
                            us</a>
                        <a href="javascript:void(0)"
                            class="focus:outline-none focus:underline hover:text-gray-500 text-base leading-4 mt-6 text-gray-800  cursor-pointer">Testimonials</a>
                    </div>
                    <div class="flex flex-col">
                        <h2 class="text-base font-semibold leading-4 text-gray-800">Support</h2>
                        <a href="javascript:void(0)"
                            class="focus:outline-none focus:underline hover:text-gray-500 text-base leading-4 mt-6 text-gray-800  cursor-pointer">Legal
                            policy</a>
                        <a href="javascript:void(0)"
                            class="focus:outline-none focus:underline hover:text-gray-500 text-base leading-4 mt-6 text-gray-800  cursor-pointer">Status
                            policy</a>
                        <a href="javascript:void(0)"
                            class="focus:outline-none focus:underline text-gray-800 text-base leading-4 mt-6 hover:text-gray-500  cursor-pointer">Privacy
                            policy</a>
                        <a href="javascript:void(0)"
                            class="focus:outline-none focus:underline hover:text-gray-500 text-base leading-4 mt-6 text-gray-800  cursor-pointer">Terms
                            of service</a>

                    </div>
                    <div class="mt-10 lg:block hidden">
                        <label class="text-xl font-medium leading-5 text-gray-800 ">Get updates</label>
                        <div
                            class="cursor-pointer flex items-center justify-between border border-gray-800 dark:border-white mt-4">
                            <input type="text"
                                class="text-base leading-4 p-4 w-full focus:outline-none text-gray-800 border-gray-800 placeholder-gray-800"
                                placeholder="Enter your email" />
                            <button aria-label="send"
                                class="mr-4 fill-current text-gray-800 hover:text-gray-500 focus:outline-none focus:ring-2 focus:ring-offset-2 focus:ring-gray-800">
                                <svg class=" dark:hover:text-gray-200" width="16" height="17" viewBox="0 0 16 17"
                                    fill="currentColor" xmlns="http://www.w3.org/2000/svg">
                                    <path
                                        d="M14.8934 7.39673L14.8884 7.39457L1.54219 1.9166C1.42993 1.87011 1.30778 1.85187 1.18666 1.86353C1.06554 1.87519 0.949225 1.91637 0.848125 1.9834C0.741311 2.05266 0.653573 2.14711 0.592805 2.25826C0.532037 2.36941 0.500145 2.49376 0.5 2.62013V6.12357C0.50006 6.29633 0.561019 6.46366 0.67237 6.59671C0.783722 6.72976 0.938491 6.82021 1.11 6.85246L8.38906 8.18438C8.41767 8.18974 8.44348 8.20482 8.46205 8.22701C8.48062 8.2492 8.49078 8.2771 8.49078 8.30591C8.49078 8.33472 8.48062 8.36263 8.46205 8.38481C8.44348 8.407 8.41767 8.42208 8.38906 8.42744L1.11031 9.75936C0.938851 9.79153 0.784092 9.88185 0.67269 10.0148C0.561288 10.1477 0.500219 10.3149 0.5 10.4876V13.9917C0.499917 14.1124 0.530111 14.2312 0.587871 14.3374C0.645632 14.4437 0.729152 14.5341 0.830938 14.6006C0.953375 14.6811 1.09706 14.7241 1.24406 14.7243C1.34626 14.7242 1.4474 14.7039 1.54156 14.6646L14.8875 9.21787L14.8934 9.21509C15.0731 9.13869 15.2262 9.01185 15.3337 8.85025C15.4413 8.68866 15.4986 8.49941 15.4986 8.30591C15.4986 8.11241 15.4413 7.92316 15.3337 7.76157C15.2262 7.59997 15.0731 7.47313 14.8934 7.39673Z"
                                        fill="currentColor" />
                                </svg>
                            </button>
                        </div>
                    </div>

                </div>
            </div>
        </footer>
    </div>


</body>

</html>

# hava-durumu
@tailwind base;
@tailwind components;
@tailwind utilities;
@import url("https://fonts.googleapis.com/css2?family=Roboto:wght@300;400;500;700;900&display=swap");
* {
  font-family: "Roboto", sans-serif;
}

.hide-scrollbar::-webkit-scrollbar {
  background-color: transparent;
  width: 0px;
}
.hide-scrollbar::-webkit-scrollbar-thumb {
  background-color: transparent;
}

.loading::after {
  content: "";
  @apply absolute bg-white top-0 left-0 right-0 bottom-0 rounded-24 flex justify-center items-center z-10 dark:bg-black text-red-400;
}

.loading:before {
  content: "";
  z-index: 20;
  position: absolute;
  top: 50%;
  left: 50%;
  transform: translate(-50%, -50%);
  margin-top: -35px;
  width: 40px;
  height: 40px;
  background-image: url(icons/loading.svg);
  background-repeat: none;
  background-position: center;
  background-size: cover;
}

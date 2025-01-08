Ada beberapa langkah untuk mengintegrasikan TailwindCSS dan Alpine.js. Saya akan menuliskannya di bawah, temen-temen yang berminat, silahkan :
Pertama, Install Tailwindcss dan Install Alpine.js
kemudian kita tinggal mengkonfigurasi bagaimana nanti tailwind dan alpine ini diinstansiasi dengan menentukan file inputnya apa dan file outputnya apa. Kita akan bekerja dengan file package.json
{
  "devDependencies": {
    "tailwindcss": "^3.4.17"
  },
  "scripts": {
    "dev": "tailwindcss -i ./src/input.css -o ./src/output.css --watch",
    "alpine": "npx esbuild ./src/alpine.js --outfile=src/output.js --bundle --minify --watch" 
  },
  "dependencies": {
    "@fortawesome/fontawesome-svg-core": "^6.7.2",
    "@fortawesome/free-brands-svg-icons": "^6.7.2",
    "@fortawesome/free-regular-svg-icons": "^6.7.2",
    "@fortawesome/free-solid-svg-icons": "^6.7.2",
    "@fortawesome/react-fontawesome": "^0.2.2",
    "alpinejs": "^3.14.8",
    "esbuild": "^0.24.2",
    "tailwind-fontawesome": "^0.7.1"
  }
}


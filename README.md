# Demo: https://grety22.github.io/cra-v18.1_tailwind-v3.0.24/
# Install latest version of create-react-app

npx create-react-app my-app

cd my-app

# Install latest version of tailwind

npm install -D tailwindcss postcss autoprefixer

npx tailwindcss init -p

## Replace content in your tailwind config file (tailwind.config.js) with this code:

module.exports = {
  content: [
    "./src/**/*.{js,jsx,ts,tsx}",
  ],
  theme: {
    extend: {},
  },
  plugins: [],
}

## Add the Tailwind directives to your CSS by copying these 3 lines into your index.css (./src/index.css):

@tailwind base;

@tailwind components;

@tailwind utilities;

# Run the app

npm run start

# gh-pages added, for deploy run :

npm run deploy

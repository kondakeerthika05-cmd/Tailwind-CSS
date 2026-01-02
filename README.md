# Tailwind-CSS
Button Styling

Rounded → light gray → hover darker → active darker

<button
  class="px-4 py-2 rounded bg-gray-200 hover:bg-gray-300 active:bg-gray-400"
>
  Click Me
</button>

2️⃣ Image with Hover Effect

Rounded + shadow + smooth zoom:

<div class="w-64">
  <img
    src="https://via.placeholder.com/300"
    class="rounded shadow-lg transition-transform duration-300 hover:scale-105"
  />
</div>

3️⃣ Responsive Heading

Text grows with screen size + gradient + bold:

<h2 class="font-bold text-xl md:text-3xl lg:text-5xl bg-gradient-to-r from-purple-500 to-blue-500 text-transparent bg-clip-text">
  Responsive Gradient Heading
</h2>

4️⃣ List Styling
<ul class="list-disc list-inside pl-5">
  <li class="hover:text-blue-600">Item One</li>
  <li class="hover:text-blue-600">Item Two</li>
  <li class="hover:text-blue-600">Item Three</li>
</ul>

5️⃣ Card Component
<div class="max-w-sm bg-white shadow-lg rounded p-4">
  <img src="https://via.placeholder.com/300" class="rounded mb-3" />

  <h3 class="text-xl font-semibold mb-2">Card Title</h3>

  <p class="text-gray-600 mb-4">
    This is a simple card description.
  </p>

  <button class="px-4 py-2 bg-blue-500 text-white rounded hover:bg-blue-600">
    Read More
  </button>
</div>

6️⃣ Table Styling

Borders + zebra rows + hover:

<table class="w-full border border-gray-300">
  <thead>
    <tr class="bg-gray-200">
      <th class="border p-2">Name</th>
      <th class="border p-2">Age</th>
      <th class="border p-2">City</th>
    </tr>
  </thead>

  <tbody>
    <tr class="odd:bg-white even:bg-gray-100 hover:bg-gray-200">
      <td class="border p-2">John</td>
      <td class="border p-2">22</td>
      <td class="border p-2">Delhi</td>
    </tr>

    <tr class="odd:bg-white even:bg-gray-100 hover:bg-gray-200">
      <td class="border p-2">Mary</td>
      <td class="border p-2">24</td>
      <td class="border p-2">Mumbai</td>
    </tr>

    <tr class="odd:bg-white even:bg-gray-100 hover:bg-gray-200">
      <td class="border p-2">Raj</td>
      <td class="border p-2">27</td>
      <td class="border p-2">Hyderabad</td>
    </tr>

    <tr class="odd:bg-white even:bg-gray-100 hover:bg-gray-200">
      <td class="border p-2">Lisa</td>
      <td class="border p-2">30</td>
      <td class="border p-2">Chennai</td>
    </tr>
  </tbody>
</table>

7️⃣ Input Form

Rounded + focus ring + styled submit button:

<form class="space-y-4 max-w-md">
  <input
    type="text"
    placeholder="Name"
    class="w-full border rounded p-2 focus:outline-none focus:ring-2 focus:ring-blue-400"
  />

  <input
    type="email"
    placeholder="Email"
    class="w-full border rounded p-2 focus:outline-none focus:ring-2 focus:ring-blue-400"
  />

  <input
    type="password"
    placeholder="Password"
    class="w-full border rounded p-2 focus:outline-none focus:ring-2 focus:ring-blue-400"
  />

  <button class="w-full bg-blue-500 text-white py-2 rounded hover:bg-blue-600">
    Submit
  </button>
</form>

8️⃣ Navigation Bar (Responsive)

Stack on small → horizontal on medium+

<nav class="bg-gray-100 p-4 flex flex-col md:flex-row gap-4 md:gap-8">
  <a href="#" class="font-semibold hover:text-blue-600">Home</a>
  <a href="#" class="font-semibold hover:text-blue-600">About</a>
  <a href="#" class="font-semibold hover:text-blue-600">Contact</a>
</nav>

9️⃣ Responsive Grid Layout (6 Cards)
<div class="grid grid-cols-1 sm:grid-cols-2 lg:grid-cols-3 gap-6">
  <div class="p-4 bg-white shadow rounded">Card 1</div>
  <div class="p-4 bg-white shadow rounded">Card 2</div>
  <div class="p-4 bg-white shadow rounded">Card 3</div>
  <div class="p-4 bg-white shadow rounded">Card 4</div>
  <div class="p-4 bg-white shadow rounded">Card 5</div>
  <div class="p-4 bg-white shadow rounded">Card 6</div>
</div>

🔟 MINI RESPONSIVE PAGE (ALL TOGETHER)

Here’s a small page that includes:

✔ Navbar
✔ Hero section
✔ Features grid
✔ Table
✔ Contact form

<!DOCTYPE html>
<html lang="en">
<head>
  <meta charset="UTF-8" />
  <meta name="viewport" content="width=device-width, initial-scale=1.0" />
  <script src="https://cdn.tailwindcss.com"></script>
  <title>Tailwind Practice</title>
</head>

<body class="bg-gray-50">

  <!-- Navbar -->
  <nav class="bg-white shadow p-4 flex flex-col md:flex-row gap-4 md:gap-8">
    <a class="font-bold" href="#">Logo</a>
    <a class="hover:text-blue-600" href="#">Home</a>
    <a class="hover:text-blue-600" href="#">Features</a>
    <a class="hover:text-blue-600" href="#">Contact</a>
  </nav>

  <!-- Hero -->
  <section class="p-6 text-center">
    <h1 class="text-2xl md:text-4xl font-bold mb-4">
      Welcome to Tailwind CSS
    </h1>

    <img
      src="https://via.placeholder.com/500"
      class="mx-auto rounded shadow-lg hover:scale-105 transition"
    />
  </section>

  <!-- Features -->
  <section class="p-6 grid grid-cols-1 md:grid-cols-3 gap-6">
    <div class="bg-white shadow rounded p-4">Feature 1</div>
    <div class="bg-white shadow rounded p-4">Feature 2</div>
    <div class="bg-white shadow rounded p-4">Feature 3</div>
  </section>

  <!-- Table Section -->
  <section class="p-6">
    <h2 class="text-xl font-bold mb-2">Users Table</h2>

    <table class="w-full border">
      <tr class="bg-gray-200">
        <th class="border p-2">Name</th>
        <th class="border p-2">Age</th>
        <th class="border p-2">City</th>
      </tr>

      <tr class="odd:bg-white even:bg-gray-100 hover:bg-gray-200">
        <td class="border p-2">John</td>
        <td class="border p-2">22</td>
        <td class="border p-2">Delhi</td>
      </tr>
      <tr class="odd:bg-white even:bg-gray-100 hover:bg-gray-200">
        <td class="border p-2">Mary</td>
        <td class="border p-2">25</td>
        <td class="border p-2">Pune</td>
      </tr>
    </table>
  </section>

  <!-- Contact Form -->
  <section class="p-6">
    <h2 class="text-xl font-bold mb-3">Contact Us</h2>

    <form class="space-y-3 max-w-md">
      <input class="w-full border p-2 rounded" placeholder="Name" />
      <input class="w-full border p-2 rounded" placeholder="Email" />
      <textarea class="w-full border p-2 rounded" placeholder="Message"></textarea>

      <button class="bg-blue-500 text-white py-2 px-4 rounded">
        Send
      </button>
    </form>
  </section>

</body>
</html>

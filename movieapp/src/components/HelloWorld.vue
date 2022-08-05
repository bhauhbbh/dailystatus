<script>
const people = [
  {
    name: 'Calvin Hawkins',
    post: 'ಬದುಕು ಜಟಕಾಬಂಡಿ, ವಿಧಿ ಅದರ ಸಾಹೇಬ ಕುದುರೆ ನೀನ್,ಅವನು ಪೇಳ್ದಂತೆ  ಪಯಣಿಗರು ಮದುವೆಗೋ ಮಸಣಕೋ ಹೋಗೆಂದಕಡೆಗೋಡು, ಪದಕುಸಿಯೆ ನೆಲವಿಹುದು ಮಂಕುತಿಮ್ಮ',
  },
  {
    name: 'Kristen Ramos',
    post: 'ಬದುಕು ಜಟಕಾಬಂಡಿ, ವಿಧಿ ಅದರ ಸಾಹೇಬ ಕುದುರೆ ನೀನ್,ಅವನು ಪೇಳ್ದಂತೆ  ಪಯಣಿಗರು ಮದುವೆಗೋ ಮಸಣಕೋ ಹೋಗೆಂದಕಡೆಗೋಡು, ಪದಕುಸಿಯೆ ನೆಲವಿಹುದು ಮಂಕುತಿಮ್ಮ',
  },
  {
    name: 'Ted Fox',
    post: 'ಬದುಕು ಜಟಕಾಬಂಡಿ, ವಿಧಿ ಅದರ ಸಾಹೇಬ ಕುದುರೆ ನೀನ್,ಅವನು ಪೇಳ್ದಂತೆ  ಪಯಣಿಗರು ಮದುವೆಗೋ ಮಸಣಕೋ ಹೋಗೆಂದಕಡೆಗೋಡು, ಪದಕುಸಿಯೆ ನೆಲವಿಹುದು ಮಂಕುತಿಮ್ಮ',
  },
];

export default {
  setup() {
    return {
      people,
    };
  },
};
</script>

<template>
  <div class="container mx-auto px-4">
    <div
      class="card w-80 bg-neutral text-neutral-content custom mt-9"
      v-for="person in people"
      :key="person.email"
    >
      <div class="card-body items-center text-center">
        <!-- <h2 class="card-title">Cookies!</h2> -->
        <p>
          {{ person.post }}
        </p>
        <!-- <div class="card-actions justify-end pt-3">
        <button class="btn btn-primary">Like</button>
        <button class="btn btn-accent">Button</button>
      </div> -->
      </div>
      <button class="btn btn-active btn-secondary gap-2">
        <svg
          xmlns="http://www.w3.org/2000/svg"
          class="h-6 w-6"
          fill="none"
          viewBox="0 0 24 24"
          stroke="currentColor"
        >
          <path
            stroke-linecap="round"
            stroke-linejoin="round"
            stroke-width="2"
            d="M4.318 6.318a4.5 4.5 0 000 6.364L12 20.364l7.682-7.682a4.5 4.5 0 00-6.364-6.364L12 7.636l-1.318-1.318a4.5 4.5 0 00-6.364 0z"
          />
        </svg>
        Button
      </button>
    </div>

    <!-- <div class="md:container md:mx-auto px-9">
      <h1>Hellow eveyone</h1>
      <ul class="divide-y divide-gray-200">
        <li v-for="person in people" :key="person.email" class="py-4 flex">
          <img class="h-10 w-10 rounded-full" :src="person.image" alt="" />
          <div class="ml-3">
            <p class="text-sm font-medium text-gray-900">{{ person.name }}</p>
            <p class="text-sm text-gray-500">{{ person.email }}</p>
          </div>
        </li>
      </ul>
    </div> -->
  </div>
</template>

<style scoped></style>

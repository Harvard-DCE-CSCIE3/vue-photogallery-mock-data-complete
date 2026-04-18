# CSCI E-31: Vue PhotoGallery Demo (Mock Data)

This is a **small Vue 3 + TypeScript demo app** for CSCI E-31. **It mirrors the end state of the Express Photo Gallery Vue App as of the end of class meeting 11.** 

It renders a photo gallery using **mock data** (no backend calls in this version), and is meant to support early Vue learning goals. It handles the RUD of CRUD (Create, Read, Update, Delete) with a simple local data service, but does not include file upload or any real persistence.

## What this project adds to the Week 10 example:

- Send information from child components back to parents with typed custom events
	- Use `defineEmits` in a child and handle the emitted event in the parent
- Add client-side routing with Vue Router for gallery, detail, and edit views
	- Use `RouterLink` for visible navigation and `router.push()` after actions
- Use route params plus `watch()` and `computed()` to keep detail/edit views in sync with the URL
- Build simple form-based editing with `v-model` and `@submit.prevent`
- Connect basic CRUD-style UI flows to a simple local data service
	- Load one photo, update title/description, and delete a photo before returning to the gallery

### Goals from the Week 10 project

- Component structure and nesting
- Passing data down with props
- TypeScript in Vue SFCs (`<script setup lang="ts">`)
- Type checking during development/build
- Practical UI basics
- Layouts using `<slot />`

## Install and run

From this project folder:

1. Install dependencies

	`npm install`

2. Start the dev server

	`npm run dev`

3. Open the URL shown in the terminal (usually http://localhost:5173)

---

## Other useful scripts

- `npm run build` → type-checks with `vue-tsc` and builds for production
- `npm run preview` → serves the production build locally

---



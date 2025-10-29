# Ex09 Event Registration Web Application
## Date:28.10.2025

## AIM:
To design, develop and deploy a web application for event registration.

## DESIGN STEPS:

### Step 1:
Create a new frame.

### Step 2:
Select any one preset size of your choice.

### Step 3:
Select the shapes you need.

### Step 4:
Import images as needed.

### Step 5:
Create pages based on your need and link them.

### Step 6:

Validate the HTML and CSS code.

### Step 6:

Publish the website in the given URL.

## DESIGN TOOL:
Figma

## CODE:
```
first page

index.jsx

import React from "react";
import image1 from "./image-1.png";
import logo1 from "./logo-1.png";

export const AndroidMedium = () => {
  return (
    <div className="bg-white overflow-hidden w-full min-w-[411px] min-h-[758px] relative">
      <img
        className="absolute top-0 left-0 w-[411px] h-[758px] aspect-[0.67] object-cover"
        alt="Image"
        src={image1}
      />

      <img
        className="absolute top-[15px] left-0 w-[411px] h-[62px] aspect-[6.65] object-cover"
        alt="Logo"
        src={logo1}
      />

      <div className="absolute top-[190px] left-7 w-[350px] [font-family:'jsMath-cmti10-cmti10',Helvetica] font-normal text-[#bf0f0f] text-2xl tracking-[0] leading-[normal]">
        unleash your talents
      </div>

      <div className="absolute top-[114px] left-[93px] w-[364px] [font-family:'Jolly_Lodger-Regular',Helvetica] font-normal text-black text-[64px] tracking-[0] leading-[normal] whitespace-nowrap">
        Drama Fest
      </div>

      <div className="absolute top-[406px] left-[109px] w-[269px] h-[187px] bg-[#ffb2b2] rounded-[134.5px/93.5px] border border-solid border-black" />

      <div className="absolute top-[465px] left-[177px] [font-family:'Julius_Sans_One-Regular',Helvetica] font-normal text-black text-[32px] tracking-[0] leading-[normal]">
        register <br />
        NOW!!
      </div>
    </div>
  );
};


tailwind.config.js

/** @type {import('tailwindcss').Config} */
module.exports = {
  content: ["./src/**/*.{html,js,ts,jsx,tsx}"],
  theme: {
    extend: {},
  },
  plugins: [],
};

tailwind.css

@tailwind components;
@tailwind utilities;

@layer components {
  .all-\[unset\] {
    all: unset;
  }
}

:root {
  --animate-spin: spin 1s linear infinite;
}

.animate-fade-in {
  animation: fade-in 1s var(--animation-delay, 0s) ease forwards;
}

.animate-fade-up {
  animation: fade-up 1s var(--animation-delay, 0s) ease forwards;
}

.animate-marquee {
  animation: marquee var(--duration) infinite linear;
}

.animate-marquee-vertical {
  animation: marquee-vertical var(--duration) linear infinite;
}

.animate-shimmer {
  animation: shimmer 8s infinite;
}

.animate-spin {
  animation: var(--animate-spin);
}

@keyframes spin {
  to {
    transform: rotate(1turn);
  }
}

@keyframes image-glow {
  0% {
    opacity: 0;
    animation-timing-function: cubic-bezier(0.74, 0.25, 0.76, 1);
  }

  10% {
    opacity: 0.7;
    animation-timing-function: cubic-bezier(0.12, 0.01, 0.08, 0.99);
  }

  to {
    opacity: 0.4;
  }
}

@keyframes fade-in {
  0% {
    opacity: 0;
    transform: translateY(-10px);
  }

  to {
    opacity: 1;
    transform: none;
  }
}

@keyframes fade-up {
  0% {
    opacity: 0;
    transform: translateY(20px);
  }

  to {
    opacity: 1;
    transform: none;
  }
}

@keyframes shimmer {
  0%,
  90%,
  to {
    background-position: calc(-100% - var(--shimmer-width)) 0;
  }

  30%,
  60% {
    background-position: calc(100% + var(--shimmer-width)) 0;
  }
}

@keyframes marquee {
  0% {
    transform: translate(0);
  }

  to {
    transform: translateX(calc(-100% - var(--gap)));
  }
}

@keyframes marquee-vertical {
  0% {
    transform: translateY(0);
  }

  to {
    transform: translateY(calc(-100% - var(--gap)));
  }
}


Second Page

index.jsx

import React from "react";
import image2 from "./image-2.png";

export const AndroidMedium = () => {
  return (
    <div className="bg-white w-full min-w-[411px] min-h-[758px] relative">
      <img
        className="absolute top-0 left-0 w-[411px] h-[758px] aspect-[0.67] object-cover"
        alt="Image"
        src={image2}
      />

      <p className="absolute top-[392px] left-14 [font-family:'Cabin-Regular',Helvetica] font-normal text-black text-xl tracking-[0] leading-[normal]">
        Stage Play
        <br />
        Mime
        <br />
        Monologue
        <br />
        Skit
        <br />
        Street Play
        <br />
        Adaptation Round
        <br />
        Costume Drama, etc.
      </p>

      <div className="absolute top-[59px] left-[61px] w-[268px] [font-family:'Julius_Sans_One-Regular',Helvetica] font-normal text-black text-[32px] tracking-[0] leading-[normal] whitespace-nowrap">
        This November..
      </div>

      <p className="absolute top-[211px] left-[13px] w-[316px] [font-family:'Cabin_Condensed-SemiBold',Helvetica] font-semibold text-black text-[32px] tracking-[0] leading-[normal]">
        step into the spotlight..
        <br />
        Become a story..
      </p>

      <p className="absolute top-[674px] left-0 [font-family:'Cabin-Regular',Helvetica] font-normal text-black text-xl tracking-[0] leading-[normal]">
        🗓 Date: 15th November 2025
        <br />🕒 Time: 5:00 PM onwards
        <br />📍 Venue: College Auditorium Hall
      </p>
    </div>
  );
};

tailwind.config.js

/** @type {import('tailwindcss').Config} */
module.exports = {
  content: ["./src/**/*.{html,js,ts,jsx,tsx}"],
  theme: {
    extend: {},
  },
  plugins: [],
};

tailwind.css

@tailwind components;
@tailwind utilities;

@layer components {
  .all-\[unset\] {
    all: unset;
  }
}

:root {
  --animate-spin: spin 1s linear infinite;
}

.animate-fade-in {
  animation: fade-in 1s var(--animation-delay, 0s) ease forwards;
}

.animate-fade-up {
  animation: fade-up 1s var(--animation-delay, 0s) ease forwards;
}

.animate-marquee {
  animation: marquee var(--duration) infinite linear;
}

.animate-marquee-vertical {
  animation: marquee-vertical var(--duration) linear infinite;
}

.animate-shimmer {
  animation: shimmer 8s infinite;
}

.animate-spin {
  animation: var(--animate-spin);
}

@keyframes spin {
  to {
    transform: rotate(1turn);
  }
}

@keyframes image-glow {
  0% {
    opacity: 0;
    animation-timing-function: cubic-bezier(0.74, 0.25, 0.76, 1);
  }

  10% {
    opacity: 0.7;
    animation-timing-function: cubic-bezier(0.12, 0.01, 0.08, 0.99);
  }

  to {
    opacity: 0.4;
  }
}

@keyframes fade-in {
  0% {
    opacity: 0;
    transform: translateY(-10px);
  }

  to {
    opacity: 1;
    transform: none;
  }
}

@keyframes fade-up {
  0% {
    opacity: 0;
    transform: translateY(20px);
  }

  to {
    opacity: 1;
    transform: none;
  }
}

@keyframes shimmer {
  0%,
  90%,
  to {
    background-position: calc(-100% - var(--shimmer-width)) 0;
  }

  30%,
  60% {
    background-position: calc(100% + var(--shimmer-width)) 0;
  }
}

@keyframes marquee {
  0% {
    transform: translate(0);
  }

  to {
    transform: translateX(calc(-100% - var(--gap)));
  }
}

@keyframes marquee-vertical {
  0% {
    transform: translateY(0);
  }

  to {
    transform: translateY(calc(-100% - var(--gap)));
  }
}


Third Page

index.jsx

import React from "react";
import image3 from "./image-3.png";

export const AndroidMedium = () => {
  return (
    <div className="bg-white overflow-hidden w-full min-w-[411px] min-h-[758px] relative">
      <img
        className="absolute top-0 left-0 w-[411px] h-[758px] aspect-[0.67] object-cover"
        alt="Image"
        src={image3}
      />

      <div className="absolute top-[61px] left-3.5 w-[9641px] mix-blend-darken [font-family:'jsMath-cmti10-cmti10',Helvetica] font-normal text-black text-4xl tracking-[0] leading-[normal]">
        Registration
        <br />
        Details&nbsp;&nbsp;&nbsp;&nbsp;Detail
      </div>

      <div className="absolute top-[39px] left-0 w-[411px] h-[116px] bg-[#d9d9d9] mix-blend-hue" />

      <div className="absolute top-[202px] left-[9px] [font-family:'jsMath-cmti10-cmti10',Helvetica] font-normal text-black text-4xl tracking-[0] leading-[normal]">
        Name:
        <br />
        Department:
        <br />
        Ref:
        <br />
        Event: no:
      </div>

      <p className="absolute top-[710px] left-[23px] [font-family:'jsMath-cmti10-Regular',Helvetica] font-normal text-black text-xl tracking-[0] leading-[normal]">
        <span className="[font-family:'jsMath-cmti10-Regular',Helvetica] font-normal text-black text-xl tracking-[0]">
          Iswarya(25016326)
        </span>

        <span className="text-4xl"> b</span>
      </p>
    </div>
  );
};

tailwind.config.js

import React from "react";
import image3 from "./image-3.png";

export const AndroidMedium = () => {
  return (
    <div className="bg-white overflow-hidden w-full min-w-[411px] min-h-[758px] relative">
      <img
        className="absolute top-0 left-0 w-[411px] h-[758px] aspect-[0.67] object-cover"
        alt="Image"
        src={image3}
      />

      <div className="absolute top-[61px] left-3.5 w-[9641px] mix-blend-darken [font-family:'jsMath-cmti10-cmti10',Helvetica] font-normal text-black text-4xl tracking-[0] leading-[normal]">
        Registration
        <br />
        Details&nbsp;&nbsp;&nbsp;&nbsp;Detail
      </div>

      <div className="absolute top-[39px] left-0 w-[411px] h-[116px] bg-[#d9d9d9] mix-blend-hue" />

      <div className="absolute top-[202px] left-[9px] [font-family:'jsMath-cmti10-cmti10',Helvetica] font-normal text-black text-4xl tracking-[0] leading-[normal]">
        Name:
        <br />
        Department:
        <br />
        Ref:
        <br />
        Event: no:
      </div>

      <p className="absolute top-[710px] left-[23px] [font-family:'jsMath-cmti10-Regular',Helvetica] font-normal text-black text-xl tracking-[0] leading-[normal]">
        <span className="[font-family:'jsMath-cmti10-Regular',Helvetica] font-normal text-black text-xl tracking-[0]">
          Iswarya(25016326)
        </span>

        <span className="text-4xl"> b</span>
      </p>
    </div>
  );
};

tailwind.css

@tailwind components;
@tailwind utilities;

@layer components {
  .all-\[unset\] {
    all: unset;
  }
}

:root {
  --animate-spin: spin 1s linear infinite;
}

.animate-fade-in {
  animation: fade-in 1s var(--animation-delay, 0s) ease forwards;
}

.animate-fade-up {
  animation: fade-up 1s var(--animation-delay, 0s) ease forwards;
}

.animate-marquee {
  animation: marquee var(--duration) infinite linear;
}

.animate-marquee-vertical {
  animation: marquee-vertical var(--duration) linear infinite;
}

.animate-shimmer {
  animation: shimmer 8s infinite;
}

.animate-spin {
  animation: var(--animate-spin);
}

@keyframes spin {
  to {
    transform: rotate(1turn);
  }
}

@keyframes image-glow {
  0% {
    opacity: 0;
    animation-timing-function: cubic-bezier(0.74, 0.25, 0.76, 1);
  }

  10% {
    opacity: 0.7;
    animation-timing-function: cubic-bezier(0.12, 0.01, 0.08, 0.99);
  }

  to {
    opacity: 0.4;
  }
}

@keyframes fade-in {
  0% {
    opacity: 0;
    transform: translateY(-10px);
  }

  to {
    opacity: 1;
    transform: none;
  }
}

@keyframes fade-up {
  0% {
    opacity: 0;
    transform: translateY(20px);
  }

  to {
    opacity: 1;
    transform: none;
  }
}

@keyframes shimmer {
  0%,
  90%,
  to {
    background-position: calc(-100% - var(--shimmer-width)) 0;
  }

  30%,
  60% {
    background-position: calc(100% + var(--shimmer-width)) 0;
  }
}

@keyframes marquee {
  0% {
    transform: translate(0);
  }

  to {
    transform: translateX(calc(-100% - var(--gap)));
  }
}

@keyframes marquee-vertical {
  0% {
    transform: translateY(0);
  }

  to {
    transform: translateY(calc(-100% - var(--gap)));
  }
}

```
## OUTPUT:
![alt text](<Screenshot 2025-10-28 115653.png>)
## RESULT:
The program to design, develop and deploy a web application for event registration is completed successfully.

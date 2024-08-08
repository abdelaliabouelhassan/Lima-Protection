<template>
  <section class="w-full h-full pb-14 px-4 xl:px-0">
    <div class="w-full mx-auto max-w-[928px]">
      <div>
        <router-link to="/blog" class="flex items-center gap-2">
          <svg
            xmlns="http://www.w3.org/2000/svg"
            fill="none"
            viewBox="0 0 24 24"
            stroke-width="1.5"
            stroke="currentColor"
            class="size-5 text-black text-opacity-35"
          >
            <path
              stroke-linecap="round"
              stroke-linejoin="round"
              d="M15.75 19.5 8.25 12l7.5-7.5"
            />
          </svg>

          <span
            class="text-black text-opacity-35 uppercase font-black font-satoshi text-sm"
            >Back to Blog</span
          >
        </router-link>
      </div>

      <div class="w-full flex flex-col items-center gap-6 pt-14 sm:pt-20">
        <span
          class="text-black text-opacity-35 uppercase font-black font-satoshi text-sm"
          >Industry Trends</span
        >

        <h1
          class="text-black font-satoshi text-3xl sm:text-5xl font-bold text-center"
        >
          The Evolution of Security Bodyguards
        </h1>

        <p
          class="text-base font-normal font-satoshi text-black text-opacity-70 text-center"
        >
          Exploring how modern technology and training have transformed the role
          of security bodyguards
        </p>
      </div>

      <div class="w-full pt-14 border-b border-black border-opacity-20 pb-10">
        <div
          class="w-full h-[300px] sm:h-[592px] bg-gray-200 rounded-3xl overflow-hidden"
        >
          <img
            src="/images/blog/blog-5.png"
            class="w-full h-full object-cover bg-[#F1F1F1] mix-blend-luminosity"
            alt=""
          />
        </div>
        <div
          class="w-full flex sm:flex-row flex-col items-center gap-4 sm:justify-between pt-6"
        >
          <div class="flex items-center gap-4">
            <div class="flex items-center gap-2">
              <div class="rounded-full w-[22px] h-[22px] bg-[#D9D9D9]"></div>
              <span class="font-normal font-satoshi text-base italic text-black"
                >Jessica A.</span
              >
            </div>
            <div
              class="w-[6px] h-[6px] rounded-full bg-black bg-opacity-20"
            ></div>
            <span class="font-normal font-satoshi text-base italic text-black"
              >24 Aug, 2024</span
            >
          </div>
          <div class="flex items-center gap-4">
            <a href="#" target="_blank">
              <svg
                width="24"
                height="25"
                viewBox="0 0 24 25"
                fill="none"
                xmlns="http://www.w3.org/2000/svg"
              >
                <path
                  d="M23.6668 12.5C23.6668 6.06004 18.4402 0.833374 12.0002 0.833374C5.56016 0.833374 0.333496 6.06004 0.333496 12.5C0.333496 18.1467 4.34683 22.8484 9.66683 23.9334V16H7.3335V12.5H9.66683V9.58337C9.66683 7.33171 11.4985 5.50004 13.7502 5.50004H16.6668V9.00004H14.3335C13.6918 9.00004 13.1668 9.52504 13.1668 10.1667V12.5H16.6668V16H13.1668V24.1084C19.0585 23.525 23.6668 18.555 23.6668 12.5Z"
                  fill="black"
                  fill-opacity="0.3"
                />
              </svg>
            </a>
            <a href="#" target="_blank">
              <svg
                width="24"
                height="23"
                viewBox="0 0 24 23"
                fill="none"
                xmlns="http://www.w3.org/2000/svg"
              >
                <path
                  fill-rule="evenodd"
                  clip-rule="evenodd"
                  d="M23.1836 22.4376L14.4366 9.6884L14.4515 9.70035L22.3382 0.562561H19.7027L13.278 8.00006L8.17598 0.562561H1.26394L9.4301 12.4656L9.42911 12.4646L0.816406 22.4376H3.45193L10.5947 14.1629L16.2716 22.4376H23.1836ZM7.13172 2.55119L19.4043 20.4489H17.3158L5.03328 2.55119H7.13172Z"
                  fill="black"
                  fill-opacity="0.3"
                />
              </svg>
            </a>
            <a href="#" target="_blank">
              <svg
                width="24"
                height="23"
                viewBox="0 0 24 23"
                fill="none"
                xmlns="http://www.w3.org/2000/svg"
              >
                <path
                  d="M0.625 1.75453C0.625 0.854483 1.37291 0.125061 2.2957 0.125061H21.7043C22.6271 0.125061 23.375 0.854483 23.375 1.75453V21.2456C23.375 22.1456 22.6271 22.8751 21.7043 22.8751H2.2957C1.37291 22.8751 0.625 22.1456 0.625 21.2456V1.75453ZM7.65333 19.1697V8.89661H4.23941V19.1697H7.65333ZM5.94708 7.49322C7.13719 7.49322 7.87798 6.7055 7.87798 5.71872C7.85666 4.71061 7.13861 3.94422 5.96983 3.94422C4.80105 3.94422 4.0375 4.71203 4.0375 5.71872C4.0375 6.7055 4.7783 7.49322 5.92433 7.49322H5.94708ZM12.9256 19.1697V13.4324C12.9256 13.1253 12.9484 12.8181 13.0394 12.5992C13.2854 11.9863 13.847 11.3508 14.7911 11.3508C16.0268 11.3508 16.5201 12.292 16.5201 13.6741V19.1697H19.9341V13.2774C19.9341 10.1208 18.2506 8.65347 16.004 8.65347C14.1925 8.65347 13.3806 9.64878 12.9256 10.3498V10.3853H12.9029L12.9256 10.3498V8.89661H9.51314C9.5558 9.86064 9.51314 19.1697 9.51314 19.1697H12.9256Z"
                  fill="black"
                  fill-opacity="0.3"
                />
              </svg>
            </a>
            <a href="#" target="_blank">
              <svg
                width="24"
                height="25"
                viewBox="0 0 24 25"
                fill="none"
                xmlns="http://www.w3.org/2000/svg"
              >
                <path
                  d="M13.1997 0.833374C14.5122 0.836874 15.1783 0.843874 15.7535 0.860207L15.9798 0.868374C16.2412 0.877707 16.499 0.889374 16.8105 0.903374C18.0518 0.961707 18.8988 1.15771 19.642 1.44587C20.412 1.74221 21.0607 2.14354 21.7093 2.79104C22.3028 3.37406 22.7619 4.07959 23.0545 4.85837C23.3427 5.60154 23.5387 6.44854 23.597 7.69104C23.611 8.00137 23.6227 8.25921 23.632 8.52171L23.639 8.74804C23.6565 9.32204 23.6635 9.98821 23.6658 11.3007L23.667 12.171V13.6994C23.6698 14.5503 23.6609 15.4013 23.6402 16.252L23.6332 16.4784C23.6238 16.7409 23.6122 16.9987 23.5982 17.309C23.5398 18.5515 23.3415 19.3974 23.0545 20.1417C22.7619 20.9205 22.3028 21.626 21.7093 22.209C21.1263 22.8025 20.4208 23.2616 19.642 23.5542C18.8988 23.8424 18.0518 24.0384 16.8105 24.0967L15.9798 24.1317L15.7535 24.1387C15.1783 24.155 14.5122 24.1632 13.1997 24.1655L12.3293 24.1667H10.8022C9.95081 24.1697 9.09945 24.1608 8.24834 24.1399L8.022 24.1329C7.74505 24.1224 7.46816 24.1103 7.19134 24.0967C5.95 24.0384 5.103 23.8424 4.35867 23.5542C3.58031 23.2614 2.87519 22.8024 2.2925 22.209C1.69861 21.6261 1.23913 20.9206 0.946172 20.1417C0.658005 19.3985 0.462005 18.5515 0.403671 17.309L0.368671 16.4784L0.362838 16.252C0.341332 15.4013 0.331609 14.5504 0.333671 13.6994V11.3007C0.330442 10.4497 0.338999 9.59877 0.359338 8.74804L0.367505 8.52171C0.376838 8.25921 0.388505 8.00137 0.402505 7.69104C0.460838 6.44854 0.656838 5.60271 0.945005 4.85837C1.23865 4.07927 1.69893 3.37372 2.29367 2.79104C2.87602 2.19785 3.58072 1.73879 4.35867 1.44587C5.103 1.15771 5.94884 0.961707 7.19134 0.903374C7.50167 0.889374 7.76067 0.877707 8.022 0.868374L8.24834 0.861374C9.09906 0.840646 9.95003 0.8317 10.801 0.834541L13.1997 0.833374ZM12.0003 6.66671C10.4532 6.66671 8.96951 7.28129 7.87555 8.37525C6.78159 9.46921 6.167 10.9529 6.167 12.5C6.167 14.0471 6.78159 15.5309 7.87555 16.6248C8.96951 17.7188 10.4532 18.3334 12.0003 18.3334C13.5474 18.3334 15.0312 17.7188 16.1251 16.6248C17.2191 15.5309 17.8337 14.0471 17.8337 12.5C17.8337 10.9529 17.2191 9.46921 16.1251 8.37525C15.0312 7.28129 13.5474 6.66671 12.0003 6.66671ZM12.0003 9.00004C12.46 8.99996 12.9151 9.09042 13.3398 9.26624C13.7644 9.44206 14.1503 9.6998 14.4754 10.0248C14.8004 10.3497 15.0583 10.7355 15.2343 11.1601C15.4102 11.5847 15.5008 12.0398 15.5009 12.4995C15.501 12.9591 15.4105 13.4142 15.2347 13.8389C15.0589 14.2636 14.8012 14.6494 14.4762 14.9745C14.1513 15.2996 13.7655 15.5574 13.3409 15.7334C12.9162 15.9094 12.4611 16 12.0015 16C11.0732 16 10.183 15.6313 9.52663 14.9749C8.87025 14.3185 8.5015 13.4283 8.5015 12.5C8.5015 11.5718 8.87025 10.6815 9.52663 10.0252C10.183 9.36879 11.0732 9.00004 12.0015 9.00004M18.1265 4.91671C17.7397 4.91671 17.3688 5.07035 17.0953 5.34384C16.8218 5.61733 16.6682 5.98827 16.6682 6.37504C16.6682 6.76181 16.8218 7.13275 17.0953 7.40624C17.3688 7.67973 17.7397 7.83337 18.1265 7.83337C18.5133 7.83337 18.8842 7.67973 19.1577 7.40624C19.4312 7.13275 19.5848 6.76181 19.5848 6.37504C19.5848 5.98827 19.4312 5.61733 19.1577 5.34384C18.8842 5.07035 18.5133 4.91671 18.1265 4.91671Z"
                  fill="black"
                  fill-opacity="0.3"
                />
              </svg>
            </a>
          </div>
        </div>
      </div>

      <div class="w-full pt-10 space-y-8">
        <p class="font-satoshi text-black font-normal text-base">
          In an ever-changing world where security concerns continue to evolve,
          the role of security bodyguards has undergone significant
          transformation. Modern technology and advanced training methods have
          revolutionized how bodyguards operate, enhancing their ability to
          protect clients effectively. This article delves into the key
          advancements that have reshaped the bodyguard industry.
        </p>

        <div class="space-y-8">
          <h2 class="text-black font-bold font-satoshi text-2xl sm:text-3xl">
            The Technological Revolution
          </h2>

          <div class="w-full space-y-2">
            <h4 class="text-black font-satoshi font-medium text-xl sm:text-2xl">
              1. Surveillance and Monitoring
            </h4>
            <p class="text-black font-satoshi font-normal">
              One of the most significant technological advancements in the
              security industry is the improvement in surveillance and
              monitoring systems. High-definition cameras, drones, and
              sophisticated software allow bodyguards to monitor environments in
              real-time, providing them with critical information to anticipate
              and mitigate potential threats.
            </p>
          </div>
          <div class="w-full space-y-2">
            <h4 class="text-black font-satoshi font-medium text-xl sm:text-2xl">
              2. Communication Systems
            </h4>
            <p class="text-black font-satoshi font-normal">
              Modern communication systems have drastically improved the
              coordination among security teams. Encrypted communication devices
              ensure secure and uninterrupted communication, allowing bodyguards
              to respond quickly and efficiently in critical situations.
            </p>
          </div>
          <div class="w-full space-y-2">
            <h4 class="text-black font-satoshi font-medium text-xl sm:text-2xl">
              3. Artificial Intelligence (AI)
            </h4>
            <p class="text-black font-satoshi font-normal">
              AI has become a game-changer in the security field. Predictive
              analytics and machine learning algorithms help bodyguards identify
              patterns and predict potential threats before they materialize.
              AI-driven facial recognition technology also aids in quickly
              identifying individuals, enhancing the security team's situational
              awareness.
            </p>
          </div>
          <div
            class="w-full h-[300px] sm:h-[592px] bg-gray-200 rounded-3xl overflow-hidden"
          >
            <img
              src="/images/blog/blog-6.png"
              class="w-full h-full object-cover bg-[#F1F1F1] mix-blend-luminosity"
              alt=""
            />
          </div>
          <h2 class="text-black font-bold font-satoshi text-2xl sm:text-3xl">
            Advanced Training Techniques
          </h2>

          <div class="w-full space-y-2">
            <h4 class="text-black font-satoshi font-medium text-xl sm:text-2xl">
              1. Scenario-Based Training
            </h4>
            <p class="text-black font-satoshi font-normal">
              Traditional training methods have evolved to include
              scenario-based training, where bodyguards are placed in realistic
              simulations to hone their skills. These scenarios help them
              practice decision-making, quick thinking, and tactical responses
              in controlled environments that mimic real-life situations.
            </p>
          </div>
          <div class="w-full space-y-2">
            <h4 class="text-black font-satoshi font-medium text-xl sm:text-2xl">
              2. Psychological Training
            </h4>
            <p class="text-black font-satoshi font-normal">
              Understanding human behavior is crucial for a bodyguard. Modern
              training programs emphasize psychological training, teaching
              bodyguards how to read body language, recognize suspicious
              behavior, and manage stressful situations effectively. This aspect
              of training enhances their ability to detect and respond to
              potential threats.
            </p>
          </div>
          <div class="w-full space-y-2">
            <h4 class="text-black font-satoshi font-medium text-xl sm:text-2xl">
              3. Specialized Skills
            </h4>
            <p class="text-black font-satoshi font-normal">
              Bodyguards today are trained in a variety of specialized skills,
              including defensive driving, first aid, and cyber security.
              Defensive driving techniques enable bodyguards to navigate through
              dangerous situations while protecting their clients. First aid
              training ensures they can provide immediate medical assistance if
              required. Cyber security training helps them protect clients from
              digital threats, which have become increasingly prevalent in the
              modern world.
            </p>
          </div>
          <div
            class="w-full h-[300px] sm:h-[592px] bg-gray-200 rounded-3xl overflow-hidden"
          >
            <img
              src="/images/blog/blog-7.png"
              class="w-full h-full object-cover bg-[#F1F1F1] mix-blend-luminosity"
              alt=""
            />
          </div>

          <div class="w-full space-y-2">
            <h2 class="text-black font-bold font-satoshi text-2xl sm:text-3xl">
              The Future of Security Bodyguards
            </h2>
            <p class="text-black font-satoshi font-normal">
              The future of the bodyguard industry looks promising, with
              continuous advancements in technology and training methods.
              Wearable technology, such as smartwatches and biometric sensors,
              is expected to play a more significant role in monitoring the
              health and stress levels of bodyguards, ensuring they remain at
              peak performance.
              <br /><br />
              Furthermore, advancements in AI and machine learning will continue
              to enhance threat detection and response capabilities. As
              technology evolves, so too will the strategies and techniques
              employed by security professionals.
            </p>
          </div>
          <div class="w-full space-y-2">
            <h2 class="text-black font-bold font-satoshi text-2xl sm:text-3xl">
              Conclusion
            </h2>
            <p class="text-black font-satoshi font-normal">
              The role of security bodyguards has evolved significantly, driven
              by technological advancements and improved training methods.
              Modern bodyguards are equipped with state-of-the-art tools and
              undergo rigorous training to protect their clients effectively. As
              technology continues to advance, the bodyguard industry will adapt
              and innovate, ensuring that the safety and security of clients
              remain paramount.
              <br /><br />
              In an increasingly complex world, the evolution of security
              bodyguards underscores the importance of staying ahead of
              potential threats. With cutting-edge technology and comprehensive
              training, today's bodyguards are better prepared than ever to
              safeguard those under their protection.
            </p>
          </div>
        </div>
      </div>
    </div>
  </section>
</template>

<script setup></script>

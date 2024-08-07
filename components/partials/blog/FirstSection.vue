<template>
  <section class="w-full h-full pb-20">
    <div
      class="w-full flex flex-col items-center pt-48 max-w-[1120px] mx-auto px-4 xl:px-0 space-y-14"
    >
      <div class="text-center max-w-[612px] mx-auto space-y-7">
        <h1 class="text-black font-bold font-satoshi text-5xl">Lima Blog</h1>
        <p
          class="text-base font-satoshi font-normal text-black text-opacity-70"
        >
          Welcome to our blog! Explore insights, trends, and expert advice on
          the world of professional security bodyguards. Stay informed and stay
          safe.
        </p>
      </div>

      <div
        class="w-full grid grid-cols-1 sm:grid-cols-2 gap-8 sm:gap-4 lg:gap-8"
      >
        <BlogCard
          title="The Evolution of Security Bodyguards"
          category="Industry Trends"
          description="Exploring how modern technology and training have transformed the role of security bodyguards"
          image="/images/blog/blog-1.png"
          size="lg"
        />
        <BlogCard
          title="Essential Skills of Bodyguards"
          category="Training & Skills"
          description="A detailed look at the critical skills required for bodyguards in today's world to avoid human errors"
          image="/images/blog/blog-2.png"
          size="lg"
        />
      </div>

      <div
        class="w-full grid grid-cols-1 sm:grid-cols-2 md:grid-cols-3 gap-8 sm:gap-4 lg:gap-8"
      >
        <BlogCard
          v-for="(blog, index, key) in blogs"
          :key="key"
          :title="blog.title"
          :category="blog.category"
          :description="blog.description"
          :image="blog.image"
          size="sm"
        />
      </div>

      <div class="w-full flex justify-center items-center">
        <button
          href="https://ax6hl0zetxi.typeform.com/to/ehMKwuTo"
          target="_blank"
          class="text-white bg-black text-base font-satoshi hover:shadow-[0px_0px_25px_rgba(255,255,255,0.5)] font-bold py-[12px] px-[24px] rounded-full duration-200"
        >
          See more posts
        </button>
      </div>
    </div>
  </section>
</template>

<script setup>
import BlogCard from "@/components/UI/BlogCard.vue";

const blogs = ref([
  {
    title: "The Importance of Hiring Professional Bodyguards",
    category: "Personal Safety",
    description:
      "Understanding the reasons why high-profile individuals invest in personal security.",
    image: "/images/blog/blog-3.png",
  },
  {
    title: "How AI is Enhancing Bodyguard Services",
    category: "Technology & Innovation",
    description:
      "Examining the impact of artificial intelligence on the effectiveness of security personnel.",
    image: "/images/blog/blog-4.png",
  },
  {
    title: "How AI is Enhancing Bodyguard Services",
    category: "Technology & Innovation",
    description:
      "Examining the impact of artificial intelligence on the effectiveness of security personnel.",
    image: "/images/blog/blog-1.png",
  },
  {
    title: "How AI is Enhancing Bodyguard Services",
    category: "Technology & Innovation",
    description:
      "Examining the impact of artificial intelligence on the effectiveness of security personnel.",
    image: "/images/blog/blog-2.png",
  },
  {
    title: "The Importance of Hiring Professional Bodyguards",
    category: "Personal Safety",
    description:
      "Understanding the reasons why high-profile individuals invest in personal security.",
    image: "/images/blog/blog-3.png",
  },
  {
    title: "How AI is Enhancing Bodyguard Services",
    category: "Technology & Innovation",
    description:
      "Examining the impact of artificial intelligence on the effectiveness of security personnel.",
    image: "/images/blog/blog-4.png",
  },
  {
    title: "How AI is Enhancing Bodyguard Services",
    category: "Technology & Innovation",
    description:
      "Examining the impact of artificial intelligence on the effectiveness of security personnel.",
    image: "/images/blog/blog-1.png",
  },
  {
    title: "How AI is Enhancing Bodyguard Services",
    category: "Technology & Innovation",
    description:
      "Examining the impact of artificial intelligence on the effectiveness of security personnel.",
    image: "/images/blog/blog-2.png",
  },
  {
    title: "How AI is Enhancing Bodyguard Services",
    category: "Technology & Innovation",
    description:
      "Examining the impact of artificial intelligence on the effectiveness of security personnel.",
    image: "/images/blog/blog-4.png",
  },
]);
</script>

<template>
  <section class="w-full pt-4 pb-20 px-4 xl:px-0">
    <div class="w-full max-w-[1120px] mx-auto space-y-4">
      <h6 class="text-black font-satoshi font-medium text-2xl">
        More related articles
      </h6>
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
]);
</script>

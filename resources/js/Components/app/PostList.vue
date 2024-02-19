<template>
    <div class="py-4 flex flex-col gap-4 h-full overflow-auto">
        <PostItem :post="post1" />
        <PostItem :post="post2" />
    </div>
</template>

<script setup>
import PostItem from "./PostItem.vue";
const post1 = {
    user: {
        id: 1,
        avatar: "https://randomuser.me/api/portraits/men/37.jpg",
        name: "John Smith",
    },
    group: null,
    attachments: [
        {
            id: 1,
            name: "test.png",
            url: "https://picsum.photos/1000",
            mime: "image/png",
        },
        {
            id: 2,
            name: "test.png",
            url: "https://picsum.photos/1000",
            mime: "image/png",
        },
        {
            id: 3,
            name: "myDocument.docx",
            url: "#",
            mime: "application/msword",
        },
    ],
    body: `
    <p>Lorem ipsum dolor sit, amet consectetur adipisicing elit. Eum corporis
        magni quis voluptatum facere! Laboriosam, impedit, suscipit corporis
        possimus, consectetur voluptate deleniti minima ducimus dolore repellat
        quaerat quod dolor maiores provident? Rerum asperiores, dolorem nostrum
        sapiente ad fuga hic alias nihil quaerat accusantium autem veniam quasi,
        magnam illum aut iste.

        Quasi expedita atque placeat quia, ab quae
        impedit quisquam voluptate asperiores, ex beatae necessitatibus,
        deleniti quam itaque nisi illo veniam dolore qui labore dolorum voluptas
        natus nostrum! Adipisci non quam iusto maxime repudiandae, aspernatur
        ut. Commodi nemo ipsa, excepturi eum facilis, cupiditate, exercitationem
        qui quas consectetur fugit cum recusandae est!</p>
  `,
    created_at: "30.01.2024",
};

const post2 = {
    user: {
        id: 1,
        avatar: "https://randomuser.me/api/portraits/men/42.jpg",
        name: "James Dean",
    },
    group: {
        id: 1,
        name: "Laravel Developers",
    },
    body: `
    <p>Lorem ipsum dolor sit, amet consectetur adipisicing elit. Eum corporis
        magni quis voluptatum facere! Laboriosam, impedit, suscipit corporis
        possimus, consectetur voluptate deleniti minima ducimus dolore repellat
        quaerat quod dolor maiores provident? Rerum asperiores, dolorem nostrum
        sapiente ad fuga hic alias nihil quaerat accusantium autem veniam quasi,
        magnam illum aut iste.

        Quasi expedita atque placeat quia, ab quae
        impedit quisquam voluptate asperiores, ex beatae necessitatibus,
        deleniti quam itaque nisi illo veniam dolore qui labore dolorum voluptas
        natus nostrum! Adipisci non quam iusto maxime repudiandae, aspernatur
        ut. Commodi nemo ipsa, excepturi eum facilis, cupiditate, exercitationem
        qui quas consectetur fugit cum recusandae est!</p>
  `,
    created_at: "30.01.2024",
};
</script>

<style lang="scss" scoped></style>

<template>
    <div class="w-full md:w-8/12 mb-20">
    <Tour/>

    <br><br><br>
        <h1 class="font-extrabold text-[32px] mb-6">The PHILADELPHIA EAGLES ANNUAL PREMIUM MEMBERSHIP REGISTRATION</h1>
        <!-- <h1 class="font-extrabold text-[32px] mb-6">The ZZ Top MEMBERSHIP CARD REGISTRATION</h1> -->
        <!-- <h1 class="font-extrabold text-[32px] mb-6">The FOO FIGHTERS MEMBERSHIP CARD REGISTRATION</h1> -->

    <div class="text-[18px]">
        <p>The PHILADELPHIA EAGLES ANNUAL PREMIUM MEMBERSHIP REGISTRATION is here. The team and its entire management have taken into consideration the acceptance of new set of fans to join the EAGLES family with unending benefits.</p>
        <!-- <p>The ZZ Top membership registration is here. The band and its management have taken into consideration the acceptance of new secondary fan members with undisputed benefits.</p> -->
        <!-- <p>The Foo Fighters membership registration is here. The band and its management have taken into consideration the acceptance of new secondary fan members with undisputed benefits.</p> -->
        <br>
        <!-- #addcard -->
        <img src="https://media.bizj.us/view/img/12067814/aaambeaglesikereesecardtruckoutside1*900xx4608-2588-0-0.jpg" alt="">
        <!-- <img src="@/assets/images/MOMC.png" alt=""> -->
        <!-- <img src="@/assets/images/zz/card.jpg" alt=""> -->
        <!-- <img src="https://shop.foofighters.com/cdn/shop/files/FFI125150.png?v=1691784927&width=533" alt=""> -->
        <br>
    </div>

        <h2 class="p-2 block font-light rounded-sm bg-black/10">Regular Price - $800.00</h2>
        <br>
        <h2 class="p-2 block font-light rounded-sm bg-black/10">Premium Price - $2,000.00</h2>

        <br><br><br>
        <h2 class="text-[32px] mb-4 font-extrabold">KNOW MORE ABOUT THE ANNUAL PREMIUM BENEFITS</h2>

        <div class="">
            <div v-for="benefit in benefits" :key="benefit.title">
                <div v-html="benefit.image"></div>
                <div class="mb-5 bg-[#004C54] text-white py-3 px-10 pb-10">
                <h2 class="font-bold text-[24px] mb-2">{{ benefit.title }}</h2>
                <p>{{ benefit.content }}</p>
                </div>
            </div>
        </div>


        <!-- <ol class="list-disc">
            <li>Personal Connection: Some memberships offer the chance to interact with the artist through virtual or in-person experiences, fostering a deeper connection between the fan and the artist.</li>
            <li>Exclusive News and Updates: Members often receive newsletters or updates directly from the artist, providing insights into their creative process and upcoming projects.</li>
            <li>Priority Updates: Members are typically the first to hear about tour dates, album releases, and other important updates, ensuring they stay in the loop.</li>
            <li>Exclusive Access: Members often get early access to concert tickets, merchandise, and new music releases, ensuring they don't miss out on their favorite artist's content.</li>
            <li>Exclusive Content: Members often gain access to behind-the-scenes content, unreleased tracks, and special performances not available to the general public.</li>
            <li>Early Ticket Access: Members typically get priority access to concert tickets, improving their chances of securing seats for in-demand shows.</li>
            <li>Meet and Greets: Some memberships include opportunities to meet the artist in person or attend exclusive fan events, creating memorable experiences.</li>
            <li>Discounts: Members may enjoy discounts on concert tickets, merchandise, and even streaming services, helping them save money on their music-related expenses.</li>
            <li>Behind-the-Scenes Content: Fans often receive behind-the-scenes content, like videos, photos, or blog posts, providing insights into the artist's creative process and personal life.</li>
            <li>Previews and Pre-releases: Fans can be the first to hear new music or see music videos before they're publicly released.</li>
            <li>Exclusive Merchandise: Members may receive exclusive, limited-edition merchandise items that are not available to non-members.</li>
            <li>Collectibles and Swag: Members may receive exclusive fan club merchandise, like limited edition posters, badges, or other collectibles.</li>
            <li>Support for the Artist: Membership fees often directly support the artist's career and projects, allowing fans to contribute to their favorite musician's success.</li>
        </ol>
        <br>
        <p>Overall, a musical fan membership enhances the fan's experience by providing unique access and perks that deepen their connection with their favorite artists or bands and by providing a range of perks and opportunities to engage more deeply with the artist and their work.</p>
        <br> -->
        <NuxtLink to="/register">
        <button class="border-[4px] border-orange-700 md:border-0 px-10 py-[10px] text-[20px] font-extrabold rounded-sm md:bg-gray-200 hover:bg-black hover:text-white"><h4>CONTINUE</h4></button>
        </NuxtLink>
    </div>
</template>

<style scoped>
sup {
    color: rgb(78, 21, 1);
    font-weight: 600;
    font-size: 20px;
}
</style>

<script>
export default {
    data() {
        return {
            benefits: [
                {
                    title: "Dedicated Service Representative",
                    content: "As a premium client, you will be connected with a dedicated service rep for year round customer service!",
                    image: `<img src='https://static.clubs.nfl.com/image/private/f_auto/eagles/nwhxy0vcogtms7o1gehh'/>`
                },
                {
                    title: "Two-Hour Early Admission",
                    content: "Premium clients will have access to their club space two hours prior to kickoff!",
                    image: `<img src='https://static.clubs.nfl.com/image/private/f_auto/eagles/reptdchwmrssysfhhgpp'/>`
                },
                {
                    title: "Exclusive Stadium Entrances",
                    content: "Premium clients will be given a dedicated VIP entrance with shorter wait times.",
                    image: `<img src='https://static.clubs.nfl.com/image/private/f_auto/eagles/vz52jjugyz4kimoqxryh'/>`
                },
                {
                    title: "Full Season Parking in VIP Lots",
                    content: "Premium Clients will have the opportunity to purchase VIP parking in some of our most exclusive lots!",
                    image: `<img src='https://static.clubs.nfl.com/image/private/f_auto/eagles/opqrp3baotu5vywvchqe'/>`
                },
                {
                    title: "Participate in Pre-Game Experiences",
                    content: "Work with your service rep to learn about pre-game experiences!",
                    image: `<img src='https://static.clubs.nfl.com/image/private/f_auto/eagles/nraf5gy3arriwajsiqrb'/>`
                },
                {
                    title: "Special Invites to Premium Events",
                    content: "Eagles fandom does not stop when the football season does! Receive invites to exclusive events year-round!",
                    image: `<img src='https://static.clubs.nfl.com/image/private/f_auto/eagles/lvrnktaltxqtotb7vozd'/>`
                },
                {
                    title: "Pro Shop Discount",
                    content: "Get 15% off when you shop in store or online using code PREM2324",
                    image: `<img src='https://static.clubs.nfl.com/image/private/f_auto/eagles/mls7bkvtkswdgxpr8kan'/>`
                },
                {
                    title: "Presale Access to Stadium Concerts and Events",
                    content: "Be the first to purchase tickets to off-season concerts and events!",
                    image: `<img src='https://static.clubs.nfl.com/image/private/f_auto/eagles/gqoin7hh8ffifvqryycr'/>`
                },
                {
                    title: "40% Discount to NFL+",
                    content: "STMS are eligible for an exclusive offer to access one year of NFL+ Premium for just $59.99",
                    image: `<img src='https://static.clubs.nfl.com/image/private/f_auto/eagles/znzjusu6j5zuxmwg6fl9'/>`
                },
            ]
        }
    },
}
</script>
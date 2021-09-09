<template>
    <div>
        <div
            style="
                text-align: center;
                font-family: ff-tisa-sans-web-pro, sans-serif;
            "
        >
            <h1 class="text">SELECT YOUR LEAGUE</h1>

            <img
                alt="cblol logo"
                src="../assets/cblol-logo.png"
                width="300"
                class="padded"
                v-on:click="league = 'cblol'"
            />

            <img
                alt="lcs logo"
                src="../assets/lcs-logo.png"
                width="150"
                height="300"
                class="padded"
                v-on:click="league = 'lcs'"
            />

            <img
                alt="lcs logo"
                src="../assets/LEC-Logo.png"
                width="300"
                class="padded"
                v-on:click="league = 'lec'"
            />

            <h2>{{ league }}</h2>
            
        </div>
    </div>
</template>

<script>
export default {
    name: "LeagueSelection",
    data: () => ({
        league: "",
    }),
};
</script>

<style>
.padded {
    padding-left: 6em;
    padding-right: 6em;
}

.padded:hover {
    border-style: dotted;
}

.text {
    color: white;
    letter-spacing: 3px;
}

.text:hover {
    text-shadow: 2px 2px 4px #000000;
}
</style>
<script lang="ts">
    export type Activity = {
        name: string;
        time: string;
        cover: string;
        paragraphs: Array<string>;
    }

    let {activity}: {activity: Activity} = $props();
</script>

<div class="activity-card">
    <div class="image" style="background-image: url({activity.cover})">
        
    </div>
    <div class="info">
        <h2 id="name">
            {activity.name}
        </h2>
        <h3 class="time">
            {activity.time}
        </h3>
        <div class="description">
            {#each activity.paragraphs as paragraph}
	            <p>
                    {paragraph}
                </p> 
            {/each}
        </div>
    </div>
</div>

<style>
    * {
        font-family: var(--font-1);
    }
    .activity-card {
        display: flex;
        flex-direction: column;
        width: 640px;
        border-radius: 1%;
        background-color: hsl(0, 0%, 15%);
    }

    #name {
        color: white;
        font-size: var(--text-3xl);
        margin-bottom: var(--spacing-2);
        line-height: 3rem;
    }

    .time {
        font-weight: 600;
        margin-bottom: var(--spacing-4);
    }

    .info {
        display: flex;
        flex-direction: column;
        margin: var(--spacing-5);
    }

    .image {
        background-size: cover;
        border-radius: 1%;
    }

    .description {
        font-size: var(--text-lg);
        line-height: 1.75rem;
    }

    @media (min-width: 768px) {
        .image {
            height: 360px;
            width: 640px;
        }
    }

    @media (max-width: 767px) {
        #name {
            font-size: var(--text-2xl);
        }

        .image {
            height: 49.5vw;
            width: 88vw;
        }

        .activity-card {
            width: 88vw;
        }
    }
    
</style>

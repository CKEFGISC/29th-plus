<script lang="ts">
    export type Slide = {
        name: string;
        link: string;
    };
    
    let { course_slide }: { course_slide: Slide } = $props();
</script>

<a href={course_slide.link} class="course-slide" target="_blank">{course_slide.name}</a>

<style>
    .course-slide {
        text-decoration: none;
    }
</style>

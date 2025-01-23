<template>
    <div v-if="$frontmatter.layout != 'cover' && $frontmatter.layout != 'intro' && $frontmatter.layout != 'credits' && $frontmatter.layout != 'full' && $frontmatter.layout != 'end'">
        <footer class="absolute bottom-0 left-0 right-0 p-2 text-sm text-gray-700 dark:text-slate-300">
            <div class="flex-col flex gap-1">
                <a href="https://github.com/lirantal" target="_blank">
                    <carbon:logo-github/> @lirantal
                </a>
            </div>
        </footer>
    </div>
</template>

<script setup>

import { useSlideContext } from '@slidev/client'
const { $slidev, $frontmatter } = useSlideContext()

</script>
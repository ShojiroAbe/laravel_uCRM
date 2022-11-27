## コンポーネーントと渡ってくる値の流れ
・pagesに変数を渡す流れは
コントローラー（Inertia::render）→ difineProps(変数) → コンポーネント
https://www.udemy.com/course/laravel-vue3-crm/learn/lecture/33278254#questions

親から子は「defineProps」（Prop down）
親->子　prop
子から親は「defineEmits」（Event up）
子->親　emit

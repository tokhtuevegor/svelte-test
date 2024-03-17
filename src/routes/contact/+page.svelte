<svelte:head>
    <title>Контакты</title>
</svelte:head>
<div class="container">
    <h1>Контакты</h1>
    <div class="contact">
        {#each routes as page}
        <div class="cont">
            <h2>{page.title}</h2>
            <p>{page.body}</p>
            <p class="clickhere">
                <a class=link href={`/contact/cont/${page.id}`}>Нажми сюда</a>
            </p>
        </div>
        {/each}
    </div>
</div>

<script>
    import {routes} from './routes'
</script>

<style>
    .container {
        margin: 20px 60px;
        max-width: 800px;
        padding: 0 20px;
    }

    .contact {
        display: grid;
        grid-template-columns: max-content;
    }

    .cont {
        border: 1px solid #ddd;
        padding: 10px;
        box-shadow: 0 0 10px #eee;
    }

    .link {
        color: rgb(255, 88, 88);
    }
    
</style>
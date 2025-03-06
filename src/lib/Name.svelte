<script lang=ts>
    let userName = $state('');
    let userNameBackwards;
    
    

</script>

<input bind:value={userName} placeholder="Enter your name" />
<p>Hello <span class='name'>{userName || 'pal'}!</span></p>

<style>
.name {
    color: red;
}
</style>

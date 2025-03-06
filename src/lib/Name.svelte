<script lang=ts>
    let userName = '';
    $:reversedName = userName.split('').reverse().join('')
    
    

</script>

<input bind:value={userName} placeholder="Enter your name" />
<p>Hello <span class='name'>{userName || 'pal'}!</span> your name backwards is <span class='nameback'>{reversedName || 'lap'}</span></p>

<style>
.name {
    color: red;
}
.nameback {
    color: blue;
}
</style>

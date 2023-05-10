<script>
    let likes = 0;
    export let date;
    export let author;
    export let text;
</script>
    <div class="wrapper">
        <div class="post">
            <div class="header">
                <div class="author">
                    {author}
                </div>
                <div class="date">
                    {date}
                </div>

            </div>
            <div class="text">
                {text}
            </div>
            <div on:click={() => {likes++}} class="like">Likes {likes}</div>
        </div>
    </div>


<style>
    .wrapper{
      font-family: Arial,serif;
      font-size: 20px;
      margin: 20px 40px;
      width: 300px;
    }
    .post{
      border: 1px solid black;
      border-radius: 40px;
      padding: 40px;
    }
    .header{
      display: flex;
      justify-content: space-between;
    }
    .text{
      margin-top: 50px;
      font-size: 18px;
      overflow: scroll;
      height: 700px;
    }
    .like{
      background-color: aqua;
      box-shadow: none;
      font-size: 14px;
      border: 1px solid black;
      padding: 5px 10px;
      margin: 20px auto;
      width: 60px;
      cursor: pointer;
      border-radius: 30px;
      text-align: center;
      user-select: none;
    }
    .like:active{
      background-color: #0fe8e8;
    }
</style>

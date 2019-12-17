<template>
  <div class="container">
    <div>
      <img src alt />
    </div>
    <div class="album" v-for="(album,index) in albums" :key="index">
      <img :src="album.imgUrl" />
      <p>
        <span>{{album.title}}</span>
        <br />
        {{album.artist}}
      </p>
    </div>
  </div>
</template>

<script>
export default {
  data() {
    return {
      albums: [
        {
          imgUrl:
            "https://img3.doubanio.com/view/subject/s/public/s24468662.jpg",
          title: "Bohemian Rhapsody - EP",
          artist: "Queen"
        },
        {
          imgUrl:
            "https://img3.doubanio.com/view/subject/s/public/s29901195.jpg",
          title: "Bohemian Rhapsody (The Original Soundtrack) 1112233",
          artist: "Queen"
        },
        {
          imgUrl:
            "https://img3.doubanio.com/view/subject/s/public/s24468665.jpg",
          title: "We Are the Champions",
          artist: "Queen"
        },
        {
          imgUrl:
            "https://img1.doubanio.com/view/subject/s/public/s9034949.jpg",
          title: "We Will Rock You - EP",
          artist: "Queen"
        },
        {
          imgUrl:
            "https://img3.doubanio.com/view/subject/s/public/s3127143.jpg",
          title: "Killer Queen",
          artist: "Queen"
        },
        {
          imgUrl:
            "https://img1.doubanio.com/view/subject/s/public/s29403358.jpg",
          title: "The Platinum Collection: Greatest Hits I, II & III",
          artist: "Queen"
        },
        {
          imgUrl:
            "https://img9.doubanio.com/view/subject/s/public/s30009524.jpg",
          title: "Bohemian Rhapsody/These Are The Days Of Our Lives",
          artist: "Queen"
        },
        {
          imgUrl:
            "https://img9.doubanio.com/view/subject/s/public/s2829956.jpg",
          title: "Greatest Hits",
          artist: "Queen"
        },
        {
          imgUrl:
            "https://img1.doubanio.com/view/subject/s/public/s4718117.jpg",
          title: "A Night at the Opera",
          artist: "Queen"
        }
      ]
    };
  }
};
</script>

<style lang="stylus" scoped>
.container
  margin 35px 0 35px 15px
  padding 10px
  background-color grey
  overflow auto 

.album
  width 280px
  height 350px
  float left
  margin-right 10px
  margin-bottom 20px
  border 2px solid #242323
  padding 5px
  background #ffffff

  img
    width 270px
    height 270px

  p
    text-align center
    font-size 15px
    color #797777

  span
    font-weight bold
    color #373737
    font-size 18px
    overflow hidden
    display inline-block
    text-overflow ellipsis 
    display -webkit-box
    -webkit-line-clamp 1
    -webkit-box-orient vertical
    word-break break-all
    width 100%
</style>
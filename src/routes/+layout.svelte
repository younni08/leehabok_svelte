<script>
    import { page } from '$app/stores';
    let path;

    $: path = $page.url.pathname;
</script>

<div class="app">

    <div class="topnavi_wrapper">
        <div class="topnavi">
            <a href="/" class="topnavi_left">
                <img src="./image/logo.png" alt="logo" />
            </a>
            <a href="/menu" class="topnavi_right2">
                <img src="./image/menu.webp" alt="logo" />
            </a>
            <div class="topnavi_right">
                <a href="/" class={path === '/' ? 'active' : ''}>
                    <span>Home</span>
                </a>
                <a href="/about" class={path === '/about' ? 'active' : ''}>
                    <span>About</span>
                </a>
                <a href="/notice" class={path === '/notice' ? 'active' : ''}>
                    <span>Notice</span>
                </a>
            </div>
        </div>
    </div>
    
    
    <slot></slot>
    
    <div class="footer">
        <div>
            <div>
                <img src="./image/company.png" alt="line" />
            </div>
            <span>copyright @ 2022 재단법인 청암문화재단 산하 민속문화재. All Rights Reserved.</span>
        </div>
    </div>
</div>


<style>
    .topnavi_wrapper{
    display: flex;
    justify-content: center;
    background: #f6f6f6;
    width: 100%;
    border-bottom: solid 1px #eee;
    }
    .topnavi_left > img{
    height: 40px;
    margin: 15px 20px 10px 20px; 
    }
    .topnavi_right2{
    display: none;
    }
    .topnavi{
    display: flex;
    justify-content: space-between;
    height: 65px;
    align-items: center;
    width:1200px;
    }
    .topnavi_right{
    display:flex;
    }
    .topnavi_right > a{
    display:flex;
    margin:0px 30px;
    color:#7f7f7f;
    cursor: pointer;
    text-decoration: none;
    }
    .topnavi_right > a.active{
    color:#964b00;
    }
    .footer{
    display:flex;
    flex-direction: column;
    justify-content: center;
    align-items: center;
    width:100%;
    /* background: #230c0e; */
    /* height:70px; */
    color:#230c0e;
    /* font-family: 'Noto Serif KR', serif; */
    font-size: 0.9rem;
    }
    .footer > div{
    display:flex;
    /* justify-content: space-between; */
    align-items: center;
    flex-direction: column;
    width: 1200px;
    margin:0px 0px 50px 0px;
    }
    .footer > div > div{
    margin:20px 0px 20px 0px;
    }
    .footer > div img{
    height:30px;
    }
    @media (min-width: 320px) and (max-width: 800px) {
    .app{
        overflow: hidden;
    }
    .topnavi_right{
        display:none;
    }
    .topnavi_right2{
        display:flex;
        padding:10px;
        width:20px;
        height:20px;
    }
    .topnavi{
        width:calc(100% - 40px);
        padding:0px 20px;
    }
    .index_lv2{
        height:100vh;
        width:auto;
    }
    .index_lv2 > div.absolute{
        display:flex;
        justify-content: center;
    }
    .index_lv2 > div.absolute > img{
        height:100vh;
        width:auto;
    }
    .index_lv2_ink{
        width:130vw;
        height: 130vw;
        margin:15vh 0px 0px 0px;
    }
    .index_lv2_ink > img:nth-child(1){
        width:100%;
        height: auto;
    }
    .index_lv3{
        overflow: visible;
        margin:0px 0px 100px 0px;
    }
    .index_lv3_3{
        display:block;
        margin:50px 0px 0px 0px;
        width:calc(100% - 40px);
    }
    .index_lv4{
        flex-direction: column;
        align-items: center;
        width:100%;
        margin:150px 0px 0px 0px;
    }
    .index_lv4 > div:first-child{
        display:flex;
        justify-content: center;
        width:calc(100% - 40px);
    }
    .index_lv4 > div:first-child > img{
        object-fit: cover;
        width:100%;
        height:100%;
    }
    .index_lv4 > div:last-child > div:first-child{
        display:flex;
        justify-content: center;
        margin:30px 0px 20px 0px;
    }
    .index_lv4 > div:last-child > div:first-child > img{
        width:50%;
    }
    .index_lv4 > div:last-child > div:nth-child(2){
        align-items: center;
        margin:0px 0px 20px 0px;
    }
    .index_lv4 > div:last-child > div:last-child{
        display:flex;
        justify-content: center;
        width:100%;
    }
    .index_lv41{
        flex-direction: column;
        align-items: center;
        width:100%;
        margin:150px 0px 0px 0px;
    }
    .index_lv41 > div:first-child{
        display:flex;
        justify-content: center;
        width:calc(100% - 40px);
    }
    .index_lv41 > div:first-child > img{
        object-fit: cover;
        width:100%;
        height:100%;
    }
    .index_lv41 > div:last-child > div:first-child{
        display:flex;
        justify-content: center;
        margin:30px 0px 20px 0px;
    }
    .index_lv41 > div:last-child > div:first-child > img{
        width:30%;
    }
    .index_lv41 > div:last-child > div:nth-child(2){
        align-items: center;
        margin:0px 0px 20px 0px;
        font-size: 1rem;
    }
    .index_lv41 > div:last-child > div:last-child{
        display:flex;
        justify-content: center;
        width:100%;
    }
    .index_lv5{
        flex-direction: column-reverse;
        align-items: center;
        width:100%;
        margin:150px 0px 0px 0px;
    }
    .index_lv5 > div:last-child{
        display:flex;
        justify-content: center;
        width:calc(100% - 40px);
    }
    .index_lv5 > div:last-child > img{
        object-fit: cover;
        width:100%;
        height:100%;
    }
    .index_lv5 > div:first-child > div:first-child{
        display:flex;
        justify-content: center;
        margin:30px 0px 20px 0px;
    }
    .index_lv5 > div:first-child > div:first-child > img{
        width:50%;
    }
    .index_lv5 > div:first-child > div:nth-child(2){
        align-items: center;
        font-size: 1rem;
        margin:0px 0px 20px 0px;
    }
    .index_lv5 > div:first-child > div:last-child{
        display:flex;
        justify-content: center;
        width:100%;
    }
    .index_lv51{
        flex-direction: column-reverse;
        align-items: center;
        width:100%;
        margin:150px 0px 0px 0px;
    }
    .index_lv51 > div:last-child{
        display:flex;
        justify-content: center;
        width:calc(100% - 40px);
    }
    .index_lv51 > div:last-child > img{
        object-fit: cover;
        width:100%;
        height:100%;
    }
    .index_lv51 > div:first-child > div:first-child{
        display:flex;
        justify-content: center;
        margin:30px 0px 20px 0px;
    }
    .index_lv51 > div:first-child > div:first-child > img{
        width:50%;
    }
    .index_lv51 > div:first-child > div:nth-child(2){
        align-items: center;
        margin:0px 0px 20px 0px;
    }
    .index_lv51 > div:first-child > div:last-child{
        display:flex;
        justify-content: center;
        width:100%;
    }
    .index_lv6{
        height:80vh;
        justify-content: center;
    }
    .index_lv6 > div{
        width:calc(100% - 40px);
        flex-direction: column;
        margin:150px 0px 0px 0px;
    }
    .index_lv6 > div > div:first-child > div{
        font-size: 1rem;
        margin:20px 0px 0px 0px;
    }
    .index_lv6 > div > div:first-child > div > img{
        width:50%;
    }
    .index_lv6 > div > div:last-child{
        width:100%;
        height: auto;
        margin:20px 0px 0px 0px;
    }
    /* -------------------------------------------------------- */
    .menu{
        display:flex;
        flex-direction: column;
        height:100vh;
        width:100%;
    }
    .menu > a{
        display: flex;
        width:calc(100% - 40px);
        padding:20px 20px;
        text-decoration: none;
        color:#7f7f7f;
        border-bottom: solid 1px #eaeaea;
    }
    .menu > a.active{
        color:#964b00;
    }
    /* -------------------------------------------------------- */
    .about{
        margin:50px 0px 0px 0px;
    }
    .about_lv1{
        flex-direction: column;
        width:calc(100% - 40px);
        padding:20px 20px;

    }
    .about_lv1 > div:first-child{
        width:100%;
        /* height: auto; */
        font-size: 2rem;
    }
    .about_lv1 > div:first-child > div{
        width:100%;
        /* height: auto; */
        margin:100px 0px 0px 50px;
    }
    .about_lv1 > div:last-child{
        flex-direction: column;
        justify-content: center;
        margin:20px 0px 0px 0px;
    }
    .about_lv1 > div:last-child > div:last-child{
        margin:20px 0px 0px 0px;
    }
    .about_lv3{
        height:50vh;
        width:calc(100% - 40px);
        padding:0px 20px;
        background-position: center;
    }
    .about_lv3 > div:first-child{
        margin:100px 0px 50px 0px;
    }
    .about_lv3 > div:last-child{
        display: block;
        font-size: 1rem;
    }
    .about_tab > div:first-child > span{
        padding:10px 5px;
        font-size: 0.8rem;
        margin:0px 10px;
    }
    .about_tab1 > div{
        width:100%;
        flex-direction: column;
    }
    .about_tab1 > div > div:first-child{
        width:calc(100% - 40px);
        padding:0px 20px;
        margin:0px 0px 50px 0px;
    }
    .about_tab1 > div > div:last-child{
        width:calc(100% - 40px);
        padding:0px 20px;
    }
    .about_tab2 > div{
        width:100%;
        flex-direction: column;
    }
    .about_tab2 > div > div:first-child{
        width:calc(100% - 40px);
        padding:0px 20px;
        margin:0px 0px 50px 0px;
    }
    .about_tab2 > div > div:last-child{
        width:calc(100% - 40px);
        padding:0px 20px;
    }
    .about_tab2 > div > div:last-child img{
        width:100%;
    }
    .about_tab2 > div > div:last-child{
        font-size: 0.8rem;
    }
    .aboutimagelist > div{
        width:100%;
    }
    .aboutimagelist > div > div:first-child{
        width:calc(100% - 40px);
        padding:0px 20px;
    }
    .aboutimagelist > div > div:first-child > img{
        width:30%;
    }
    .about_tab4 > div{
        width:calc(100% - 40px);
        padding:0px 20px;
        
    }
    .about_tab4 > div > img{
        width: 100%;
        height: auto;
    }
    .notice{
        padding:50px 0px 0px 0px;
    }
    .notice_lv1{
        flex-direction: column;
        width:calc(100% - 40px);
        padding:20px 20px;
    }
    .notice_lv1 > div:first-child{
        width:100%;
        /* height: auto; */
    }
    .notice_lv1 > div:first-child > div{
        width:100%;
        margin:100px 0px 0px 30px;
    }
    .notice_lv1 > div:first-child > div img{
        width:50%;
    }
    .about_lv1 > div:last-child{
        flex-direction: column;
        justify-content: center;
        margin:20px 0px 0px 0px;
    }
    .about_lv1 > div:last-child > div:last-child{
        margin:20px 0px 0px 0px;
    }
    .notice_lv1 > div:last-child > img{
        width:100%;
    }
    .notice_tab1{
        width:calc(100% - 40px);
        padding:20px 20px;
    }
    .notice_tab1 > div > div > div:first-child{
        height: 200px;
    }
    .notice_tab1 > div > div > span:nth-child(2){
        font-size: 0.8rem;
    }
    .notice_tab1 > div > div > span:nth-child(3){
        font-size: 0.8rem;
    }
    .notice_tour{
        width:calc(100% - 40px);
        padding:0px 20px;
    }
    .notice_tour > div{
        font-size: 1.3rem;
    }
    .notice_tour img{
        width:30%;
    }
    .notice_tab2{
        width:calc(100% - 40px);
        padding:0px 20px 50px 20px;
    }
    .notice_tab2 > div > div{
        font-size: 0.8rem;
    }
}
@media (min-width: 800px) and (max-width: 1200px) {
    .index_lv4 > div:first-child > img{
        width:400px;
        height: 300px;
    }
    .index_lv6 > div{
        width:calc(100% - 40px);
        padding:0px 20px;
    }
    .notice_lv1,.index_lv4,.index_lv41{
        padding:0px 20px;
        width:calc(100% - 40px);
    }
    .index_lv5{
        width:calc(100% - 40px);
        padding:0px 20px;
    }
    .index_lv5 > div:last-child > img{
        width:400px;
        height: 300px;
    }
    .index_lv6{
        margin:100px 0px 0px 0px;
    }
    .index_lv6 > div > div:last-child{
        width:400px;
        height: 300px;
    }
    .index_lv41 > div:first-child > img{
        width:400px;
        height: 300px;
    }
}
</style>
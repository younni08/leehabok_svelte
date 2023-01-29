<div class="index">
    <div class="index_lv2">
            <div class="index_lv2_ink">
                <img src="./image/test7.webp" alt="background" />
            </div>
        <div class="absolute">
            <img src="./image/eee.webp" alt="leehabok house" />
        </div>
    </div>
    <div class="index_lv3">
        <div class="index_lv3_1">
                <span>'함부로 나뭇가지를 치지 마라.'</span>
                <span>- 청암 이하복 선생</span>
        </div>
        <div class="index_lv3_2">
                <img src="./image/line.svg" alt="line" />
        </div>
        <div class="index_lv3_3">
                <span>충남 서천군 기산면 신산리에 위치한 서천 이하복 고택은 우리나라 중부지방의 전통농가 형태를</span>
                <span>그래도 간진하 채 보존하고 있는 대표적인 가옥으로서 그 가치를 인정 받아</span>
                <span>1984년 12월 24일 국가 민속문화재 지정받았습니다.</span>
        </div>
    </div>
    <div class="index_lv4">
        <div>
            <img src="./image/index_ad1.jpg" alt="line" />
        </div>
        <div>
            <div>
                    <span>행사</span>
                    <img src="./image/temp3.svg" alt="line" />
            </div>
            <div>
                    <span>서천에서 만나는 인생사진</span>
                    <span>우리 사랑채, 우리사랑을 채우다</span>
            </div>
            <div>
                    <img onClick={()=>{window.location.href = "http://www.seocheon.go.kr.dj3.ncsfda.org/tour.do";}} src="./image/next.png" alt="line" />
            </div>
        </div>
    </div>
    <div class="index_lv5">
        <div>
        <div>
                <span>주변 관광지</span>
                <img src="./image/temp3.svg" alt="line" />
            </div>
            <div>
                    <span>우리의 전통 문화와 자연의 소중함</span>
                    <span>서천식물예술원</span>
            </div>
            <div>
                    <img onClick={()=>{window.location.href = "http://www.seocheon.go.kr.dj3.ncsfda.org/tour.do";}} src="./image/next.png" alt="line" />
            </div>
        </div>
        <div>
            <img src="./image/index_ad2.jpg" alt="line" />
        </div>
    </div>
    <div class="index_lv4">
        <div>
            <img src="./image/index_ad3.webp" alt="line" />
        </div>
        <div>
            <div>
                    <span>사진 더보기</span>
                    <img src="./image/temp3.svg" alt="line" />
            </div>
            <div>
                    <span>청암 이하복, 고택을 이야기하다</span>
            </div>
            <div>
                    <img onClick={()=>{window.location.href = "http://www.seocheon.go.kr.dj3.ncsfda.org/tour.do";}} src="./image/next.png" alt="line" />
            </div>
        </div>
    </div>
    <div class="index_lv6">
        <div>
            <div>
                    <div>
                        <span>방문 문의</span>
                        <img src="./image/temp3.svg" alt="line" />
                    </div>
                    <div>
                        <span>문의 및 안내</span>
                        <span>041-951-3610</span>
                    </div>
                    <div>
                        <span>이용 시간</span>
                        <span>9:00 ~ 18:00</span>
                    </div>
                    <div>
                        <span>주소</span>
                        <span>충청남도 서천군 기산면 신막로 57번길 32-3</span>
                    </div>
                    <div>
                        <span class="info">이곳은 사유지로 방문시 사전 연락을 하셔야 내부를 볼 수 있습니다.</span>
                    </div>
            </div>
                <div>
                    <img src="./image/seocheonmap.png" alt="line" />
                </div>
        </div>
    </div>
</div>

<style>
/* -------------------------------------------------------- */
.index{
  display:flex;
  flex-direction: column;
  width:100%;
  align-items: center;
  position:relative;
}
/* -------------------------------------------------------- */
.index_lv2{
  display:flex;
  width: 100%;
  position:relative;
  height: auto;
  height:57.6vw;
  overflow: hidden;;
}
.index_lv2 > div.absolute{
  position:absolute;
  width:100%;
}
.index_lv2 > div.absolute > img{
  width:100%;
}
.index_lv2_ink{
  display: flex;
  z-index: 10;
  height: 550px;
  width: 550px;
  margin:10% 0px 0px 10%;
}
.index_lv2_ink > img:nth-child(1){
  width:550px;
}
/* -------------------------------------------------------- */
.index_lv3{
  display:flex;
  flex-direction: column;
  align-items: center;
  width: 100%;
  height:35.8vw;
  overflow: hidden;
  background-image: url('./image/temp4.svg');
}
.index_lv3_1{
  display:flex;
  flex-direction: column;
  align-items: center;
  margin:8vw 0px 5vw 0px;
  color:#7f7f7f;
  font-family: 'Noto Serif KR', serif;
}
.index_lv3_3{
  display:flex;
  flex-direction: column;
  align-items: center;
  color:#7f7f7f;
  margin:5vw 0px 0px 0px;
  font-family: 'Noto Serif KR', serif;
}
/* -------------------------------------------------------- */
.index_lv4{
  display:flex;
  max-width:1200px;
  width:100%;
  justify-content: space-between;
  margin:130px 0px 0px 0px;
}
.index_lv4 > div:first-child{
  display:flex;
  justify-content: center;
  align-items: center;
}
.index_lv4 > div:first-child > img{
  width:600px;
  height:400px;
}
.index_lv4 > div:last-child{
  display:flex;
  flex-direction: column;
  justify-content: space-between;
}
.index_lv4 > div:last-child > div:first-child {
  display:flex;
  align-items: center;
  margin:0px 0px 20px 0px;
}

.index_lv4 > div:last-child > div:first-child > span{
  display:flex;
  font-size: 1.5rem;
  margin:0px 20px 0px 0px;
  color:#964b00;
  font-family: 'Noto Serif KR', serif;
}
.index_lv4 > div:last-child > div:nth-child(2){
  display: flex;
  flex-direction: column;
  font-size: 1.5rem;
  font-family: 'Noto Serif KR', serif;
  color:#7f7f7f;
}
.index_lv4 > div:last-child > div:nth-child(3) img{
  cursor: pointer;
}
/* -------------------------------------------------------- */
.index_lv5{
  display:flex;
  width:1200px;
  justify-content: space-between;
  margin:130px 0px 0px 0px;
}
.index_lv5 > div:last-child{
  display:flex;
  justify-content: center;
  align-items: center;
}
.index_lv5 > div:last-child > img{
  width:600px;
  height:400px;
}
.index_lv5 > div:first-child{
  display:flex;
  flex-direction: column;
  justify-content: space-between;
}
.index_lv5 > div:first-child > div:first-child {
  display:flex;
  align-items: center;
  margin:0px 0px 20px 0px;
}
.index_lv5 > div:first-child > div:first-child > span{
  display:flex;
  font-size: 1.5rem;
  margin:0px 20px 0px 0px;
  color:#964b00;
  font-family: 'Noto Serif KR', serif;
}
.index_lv5 > div:first-child > div:nth-child(2){
  display: flex;
  flex-direction: column;
  font-size: 1.5rem;
  font-family: 'Noto Serif KR', serif;
  color:#7f7f7f;
}
.index_lv5 > div:first-child > div:nth-child(3) img{
  cursor: pointer;
}
/* -------------------------------------------------------- */
.index_lv6{
  display:flex;
  justify-content: center;
  width: 100%;
  height:41.6vw;
  overflow: hidden;
  margin:50px 0px 0px 0px;
  background-image: url('./image/footer.jpg');
  background-size: cover;
}
.index_lv6 > div{
  display:flex;
  width:1200px;
  justify-content: space-between;
  padding:13vw 0px 5vw 0px;
}
.index_lv6 > div > div:first-child{
  display: flex;
  flex-direction: column;
}
.index_lv6 > div > div:first-child > div:nth-child(1){
  display:flex;
  align-items: center;
  margin:0px 0px 20px 0px;
}
.index_lv6 > div > div:first-child > div:nth-child(1) > span{
  display:flex;
  font-size: 1.5rem;
  margin:0px 20px 0px 0px;
  color:#964b00;
  font-family: 'Noto Serif KR', serif;
}
.index_lv6 > div > div:first-child > div{
  display:flex;
  font-size: 1.3rem;
  margin:50px 0px 0px 0px;
  color:#7f7f7f;
  font-family: 'Noto Serif KR', serif;
}
.index_lv6 > div > div:first-child > div > span:first-child{
  display: flex;
  margin:0px 20px 0px 0px;
}
.index_lv6 > div > div:last-child{
  display:flex;
  justify-content: center;
  align-items: center;
  width: 600px;
  height: 400px;
  overflow: hidden;
  border-radius: 10px;
}
.index_lv6 > div > div:last-child > img{
  object-fit: cover;
}
.index_lv6 > div > div:first-child > div > span.info{
  margin:0px;
  font-size: 1rem;
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

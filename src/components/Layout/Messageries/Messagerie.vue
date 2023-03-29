<template>
  <div class="row text_zon p-0 m-0 position">
    <div class="col-1 tools_bar  overflow-auto p-0 m-0">
      <div class="mt-5 tools_btns ">
      <router-link to="/" class="d-block mx-2 my-0 p-2 sticky-top" style="margin-bottom:250px !important">
          <button class="btn  tools_btn p-0 "><img class="" src="data:image/png;base64,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" alt="oppppsss" data-v-fcfae250="">  </button>
      </router-link>
        <div class="d-block mx-3 my-5 p-1">
          <button class="btn  tools_btn  "><di class="bi bi-people"></di></button>
        </div>
        <div class="d-block mx-3 my-5 p-1">
          <button class="btn  tools_btn  "><di class="bi bi-chat-left"></di></button>
        </div>
        <div class="d-block mx-3 my-5 p-1">
          <button class="btn  tools_btn  "><di class="bi bi-bell"></di></button>
        </div>
        <div class="d-block mx-3 my-5 p-1">
          <button class="btn  tools_btn  "><di class="bi bi-person"></di></button>
        </div>
        <div class="d-block mx-3 my-5 p-1">
          <button class="btn  tools_btn  "><di class="bi bi-person"></di></button>
        </div>
        <div class="d-block mx-3 my-5 p-1">
          <button class="btn  tools_btn  "><di class="bi bi-person"></di></button>
        </div>
        <div class="d-block mx-3 my-5 p-1">
          <button class="btn  tools_btn  "><div class="bi bi-gear"></div></button>
        </div>
      </div>
    </div>
    <div class="col-11 p-0">
      <div class="messaging ">
            <div class="inbox_msg">
              <div class="inbox_people">
                <div class="headind_srch row sticky-top1">
                  <div class="recent_heading col-12 p-1 text-light">
                    <h4>Recent</h4>
                  </div>
                  <div class="srch_bar col-12 mt-2">
                    <div class="stylish-input-group p-1 row">
                      <input type="text " class="search-bar text-light col-10"  placeholder="Search" >
                      <button type="button" class="btn text-light rounded-circle col-2"> <i class="bi bi-search" aria-hidden="true"></i> </button>
                    </div>
                  </div>
                </div>
                <div class="inbox_chat">
                  <div class="chat_list  active_chat">
                    <div class="chat_people">
                      <div class="chat_img"> <img class="img-rounded" src="@/assets/img/BreakingBad4.png" alt="sunil"> </div>
                      <div class="chat_ib">
                        <h5>Sunil Rajput <span class="chat_date">Dec 25</span></h5>
                        <p>Test, which is a new approach to have all solutions 
                          astrology under one roof.</p>
                      </div>
                    </div>
                  </div>
                  <div class="chat_list ">
                    <div class="chat_people">
                      <div class="chat_img"> <img class="img-rounded" src="@/assets/img/BreakingBad4.png" alt="sunil"> </div>
                      <div class="chat_ib">
                        <h5>Sunil Rajput <span class="chat_date">Dec 25</span></h5>
                        <p>Test, which .</p>
                      </div>
                    </div>
                  </div>
                  <div class="chat_list">
                    <div class="chat_people">
                      <div class="chat_img"> <img class="img-rounded" src="@/assets/img/BreakingBad4.png" alt="sunil"> </div>
                      <div class="chat_ib">
                        <h5>Sunil Rajput <span class="chat_date">Dec 25</span></h5>
                        <p>Test, which is a new approach to have all solutions 
                          astrology under one roof.</p>
                      </div>
                    </div>
                  </div>
                  <div class="chat_list">
                    <div class="chat_people">
                      <div class="chat_img"> <img class="img-rounded" src="@/assets/img/BreakingBad4.png" alt="sunil"> </div>
                      <div class="chat_ib">
                        <h5>Sunil Rajput <span class="chat_date">Dec 25</span></h5>
                        <p>Test, which is a new approach to have all solutions 
                          astrology under one roof.</p>
                      </div>
                    </div>
                  </div>
                  <div class="chat_list ">
                    <div class="chat_people">
                      <div class="chat_img"> <img class="img-rounded" src="@/assets/img/BreakingBad4.png" alt="sunil"> </div>
                      <div class="chat_ib">
                        <h5>Sunil Rajput <span class="chat_date">Dec 25</span></h5>
                        <p>Test, which is a new approach to have all solutions 
                          astrology under one roof.</p>
                      </div>
                    </div>
                  </div>
                  <div class="chat_list">
                    <div class="chat_people">
                      <div class="chat_img"> <img class="img-rounded" src="@/assets/img/BreakingBad4.png" alt="sunil"> </div>
                      <div class="chat_ib">
                        <h5>Sunil Rajput <span class="chat_date">Dec 25</span></h5>
                        <p>Test, which is a new approach to have all solutions 
                          astrology under one roof.</p>
                      </div>
                    </div>
                  </div>
                  <div class="chat_list">
                    <div class="chat_people">
                      <div class="chat_img"> <img class="img-rounded" src="@/assets/img/BreakingBad4.png" alt="sunil"> </div>
                      <div class="chat_ib">
                        <h5>Sunil Rajput <span class="chat_date">Dec 25</span></h5>
                        <p>Test, which is a new approach to have all solutions 
                          astrology under one roof.</p>
                      </div>
                    </div>
                  </div>
                </div>
              </div>
              <div class="mesgs">
                <div class="msg_history">
                  <div class="incoming_msg">
                    <div class="incoming_msg_img"> <img class="img-rounded" src="@/assets/img/BreakingBad4.png" alt="sunil"> </div>
                    <div class="received_msg">
                      <div class="received_withd_msg">
                        <p>Test which is a new approach to have all
                          solutions</p>
                        <span class="time_date"> 11:01 AM    |    June 9</span></div>
                    </div>
                  </div>
                  <div class="outgoing_msg">
                    <div class=" d-flex justify-content-end">
                      <div class="sent_msg d-inline-block">
                        <p>Test which is a new approach to have all
                          solutions</p>
                        <span class="time_date"> 11:01 AM    |    June 9</span> </div>
                      <div class="incoming_msg_img float-end"> <img class="img-rounded" src="@/assets/img/BreakingBad4.png" alt="sunil"> </div>
                    </div>
                  </div>
                  <div class="incoming_msg">
                    <div class="incoming_msg_img"> <img class="img-rounded" src="@/assets/img/BreakingBad4.png" alt="sunil"> </div>
                    <div class="received_msg">
                      <div class="received_withd_msg">
                        <p>Test, which is a new approach to have</p>
                        <span class="time_date"> 11:01 AM    |    Yesterday</span></div>
                    </div>
                  </div>
                  <div class="outgoing_msg">
                    <div class=" d-flex justify-content-end">
                      <div class="sent_msg d-inline-block">
                        <p>Test which is a new approach to have all
                          solutions</p>
                        <span class="time_date"> 11:01 AM    |    June 9</span> </div>
                      <div class="incoming_msg_img float-end"> <img class="img-rounded" src="@/assets/img/BreakingBad4.png" alt="sunil"> </div>
                    </div>
                  </div>
                  <div class="incoming_msg">
                    <div class="incoming_msg_img"> <img class="img-rounded" src="@/assets/img/BreakingBad4.png" alt="sunil"> </div>
                    <div class="received_msg">
                      <div class="received_withd_msg">
                        <p>We work directly with our designers and suppliers,
                          and sell direct to you, which means quality, exclusive
                          products, at a price anyone can afford.</p>
                        <span class="time_date"> 11:01 AM    |    Today</span>
                      </div>
                    </div>
                  </div>
                  <div class="outgoing_msg">
                    <div class=" d-flex justify-content-end">
                      <div class="sent_msg d-inline-block">
                        <p>Test which is a new approach to have all
                          solutions</p>
                        <span class="time_date"> 11:01 AM    |    June 9</span> </div>
                      <div class="incoming_msg_img float-end"> <img class="img-rounded" src="@/assets/img/BreakingBad4.png" alt="sunil"> </div>
                    </div>
                  </div>
                  <div class="incoming_msg">
                    <div class="incoming_msg_img"> <img class="img-rounded" src="@/assets/img/BreakingBad4.png" alt="sunil"> </div>
                    <div class="received_msg">
                      <div class="received_withd_msg">
                        <p>We work directly with our designers and suppliers,
                          and sell direct to you, which means quality, exclusive
                          products, at a price anyone can afford.</p>
                        <span class="time_date"> 11:01 AM    |    Today</span>
                      </div>
                    </div>
                  </div>
                  <div class="outgoing_msg">
                    <div class=" d-flex justify-content-end">
                      <div class="sent_msg d-inline-block">
                        <p>Test which is a new approach to have all
                          solutions</p>
                        <span class="time_date"> 11:01 AM    |    June 9</span> </div>
                      <div class="incoming_msg_img float-end"> <img class="img-rounded" src="@/assets/img/BreakingBad4.png" alt="sunil"> </div>
                    </div>
                  </div>
                  <div class="incoming_msg">
                    <div class="incoming_msg_img"> <img class="img-rounded" src="@/assets/img/BreakingBad4.png" alt="sunil"> </div>
                    <div class="received_msg">
                      <div class="received_withd_msg">
                        <p>We work directly with our designers and suppliers,
                          and sell direct to you, which means quality, exclusive
                          products, at a price anyone can afford.</p>
                        <span class="time_date"> 11:01 AM    |    Today</span>
                      </div>
                    </div>
                  </div>
                </div>
                  <div class=" down_bar p-0 mb-3 ">
                    <div class="type_msg ps-3 pe-0 ">
                      <div class="input_msg_write row ">
                        <div class="col-1 pt-2 px-0">
                          <button class="btn   rounded-circle"><i class="bi bi-emoji-smile"></i></button>
                        </div>
                        <div class="col-9 pt-2 px-0">
                          <input type="text" class="form-control1 d-inline-block " id="validationDefault01" placeholder="Saisir votre message ici ..." >
                        </div>
                        <div class="col-1 pt-2 px-0">
                          <button class="btn  rounded-circle"><i class="bi bi-paperclip"></i></button>
                        </div>
                        <div class="col-1 pt-2 px-0">
                          <button class="btn   btn-primary send_btn rounded-circle"><i class="bi bi-send"></i></button>
                        </div>
                      </div>
                      
                  </div>                
              </div>
            </div>          
          </div>
        </div>
      </div>
      </div>
      
</template>
<style scoped>


.text_zon{
  width: auto;
}
.down_bar{
  width: 108%;
  background: #000000;
  height: 60px;
  position: relative;
  bottom: -59px;
  left: -18px;
  }
.container{}
img{ max-width:100%;}
.inbox_people {
 /* background:  linear-gradient(to  right, rgb(0, 0, 0), rgba(252, 203, 144, 1));
  background: -webkit-linear-gradient(to  right rgb(0, 0, 0), rgba(252, 203, 144, 1));*/
  background-color: rgb(27, 27, 27);
  float: left;
  width: 30%; 
  height:660px;
  scrollbar-width: none;
  overflow-y: auto;
  overflow-x: hidden;
  overflow-y: scroll;

}
.inbox_msg {
  clear: both;
  overflow: hidden;
  
}
.top_spac{ margin: 20px 0 0;}


.recent_heading {
  float: left;
  border-radius: 0px 0px 50px 50px;
  background:  linear-gradient(to  right,   rgb(27, 27, 27),rgb(43, 42, 42));
  background: -webkit-linear-gradient(to  right, rgb(63, 63, 63), rgb(0, 0, 0));
  font-size: 16px;
  
}
.srch_bar {
  display: inline-block;
  text-align: right;
  border-radius: 50px 50px 50px 50px ;
  color: #c7c5c5;
  background: #0f0f0f;
}
.headind_srch{ padding:10px 29px 10px 20px; overflow:hidden; }

.recent_heading h4 {
  
  font-size: 21px;
  margin: auto;
}
.srch_bar input{ border:none; width:80%; padding:2px 0 4px 6px; background:none;}
.srch_bar .input-group-addon button {
  background: rgba(0, 0, 0, 0) none repeat scroll 0 0;
  border: medium none;
  padding: 0;
  color: #707070;
  font-size: 18px;
}
.srch_bar .input-group-addon { margin: 0 0 0 -27px;}

.chat_ib h5{ font-size:15px; color:#ffffff; margin:0 0 8px 0;}
.chat_ib h5 span{ font-size:13px; float:right;}
.chat_ib p{ font-size:14px; color:#cacaca; margin:auto}
.chat_img {
  float: left;
  width: 11%;
}
.chat_ib {
  float: left;
  padding: 0 0 0 15px;
  width: 88%;
}

.chat_people{ overflow:hidden; clear:both;}
.chat_list {
 
  margin: 0 ;
  background: #000000;
  margin:1rem !important;
  border-radius:16px 16px 16px 16px ;
  padding: .5rem !important;
}
.inbox_chat { 
  
  
  }

.active_chat{ 
  background:#6b6b6b;
  color:white;
}

.incoming_msg_img {
  display: inline-block;
  width: 8%;

}
.outgoing_msg_img {
  display: inline-block;
  width: 6%;
}
.received_msg {
  display: inline-block;
  padding: 0 0 0 1px;
  vertical-align: top;
  width: 92%;
 }
 .img-rounded{
  border-radius: 30px 30px 30px 30px;
 }
 .received_withd_msg p {
  background: #18335c none repeat scroll 0 0;
  border-radius: 3px;
  color: #646464;
  font-size: 14px;
  margin: 0;
  padding: 1px 2px 1px 2px;
  width: 100%;
}
.time_date {
  color: #747474;
  display: block;
  font-size: 12px;
  margin: 8px 0 0;
}
.received_withd_msg { width: 57%;}
.mesgs {
  float: left;
  padding: 30px 15px 0 25px;
  width: 70%;
  height: 660px;
  background: black;
  
}

 .sent_msg p {
  background: #05728f none repeat scroll 0 0;
  border-radius: 3px;
  font-size: 14px;
  margin: 0; color:#fff;
  padding: 5px 10px 5px 12px;
  width:100%;
  
}
.outgoing_msg{ overflow:hidden; margin:26px 0 26px;}
.sent_msg {
 /* float: right;*/
  width: 60%;
}
.input_msg_write input {
  background: rgba(0, 0, 0, 0) none repeat scroll 0 0;
  border:none;
  color: #8f8e8e;
  font-size: 15px;
  width: -moz-available;
}

.type_msg {
  border-top: 1px  #c4c4c4;
  width: 100%;
  

}
.chat_tools{
  width: 40%;
}
.msg_send_btn {
  background: #05728f none repeat scroll 0 0;
  border: medium none;
  border-radius: 50%;
  color: #fff;
  cursor: pointer;
  font-size: 17px;
  height: 33px;
  width: 33px;
}
.messaging { padding: 0 0 0 0;}
.msg_history {
  height: 500px;
  overflow-y: scroll;
  scrollbar-width: none;
  scrollbar-color: #cfbcaa transparent;
}
.tools_bar{
  background:  linear-gradient(to  left, rgb(0, 0, 0), rgb(0, 0, 0));
  background: -webkit-linear-gradient(to  right, rgb(37, 37, 37), rgb(190, 183, 183));
  height: 660px;
  overflow-y: scroll;
  scrollbar-width: none;
  scrollbar-color: #cfbcaa transparent;
  
}
.tools_btns{

}
.tools_btn{
  color: #cdcdcd;
}
.tools_btn:hover{
  color: #eeeeee;
  background: #464646;
}

.msg_type_zone{
  width: 93%;
}
.input_msg_write{
  background-color: rgb(27, 27, 27);
  width: 97%;
  border-radius: 50px 50px 50px 50px ;
  height: 55px;
  
  padding-top: 2px;
}
.input-group-text{
  
  background: #18335c;
  border: none;
  border-radius: 100% 100% 100% 100% !important;
  color:#cdcdcd
}
.msg_input{
  border-radius:50px 50px 50px 50px ;
}
.send_btn{
  border-radius:100px 100px  100px  100px ;
 
}
.btn {
  color:#c4c4c4
}
.form-control1{
  display: block;
  padding: .375rem .75rem;
  font-size: 1rem;
  font-weight: 400;
  line-height: 1.5; 
  background-clip: padding-box;
  -webkit-appearance: none;
  -moz-appearance: none;
  appearance: none;
  border-radius: .375rem;
  transition: border-color .15s ease-in-out,box-shadow .15s ease-in-out;
  
}
.sticky-top1 {
  position: sticky;
  top: -42px;
  z-index: 1020;
}
.position{
  position: fixed;
  top:0px
}
</style>
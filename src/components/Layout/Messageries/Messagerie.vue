<template>
  <div class="row text_zon p-0 m-0 position">
    <div class="col-1 tools_bar  overflow-auto p-0 m-0">
      <div class="mt-5 tools_btns ">
      <router-link to="/" class="btn  d-block mx-2 my-0 p-2 sticky-top" style="margin-bottom:250px !important">
          <div class=" tools_btn p-0 "><img class="" src="" alt="oppppsss">  </div>
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
/*@import url('@/assets/css/main.css');*/
</style>
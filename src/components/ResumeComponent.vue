<template>
    <div id="resume">
        <h6 class="heading">Resume</h6>
        <div class="container">
            <div data-aos="zoom-in-up" class="timeline">
                <ul v-for="item in resume" :key="item">
                    <li>
                        <span data-aos="fade-right">{{ item.year }}</span>
                        <div class="content">
                            <h3 data-aos="fade-left">{{ item.institution }}</h3>
                            <p data-aos="fade-up">
                               <b> {{ item.description }}</b>
                            </p>
                        </div>
                    </li>
                </ul>
            </div>
        </div>
        <br>
            <div class="container">
                <div class="row">
                  <div class="col-sm-6">
                    <b>Technical Skills</b>
                    <br><br>
                        <div data-aos="zoom-out-up" class="row row-cols-1 align-items-start">
                          <div class="col"><i class="bi bi-filetype-html"></i></div>
                          <div class="col"><i class="bi bi-filetype-css"></i></div>
                          <div class="col"><i class="bi bi-filetype-js"></i></div>
                          <div class="col"><i class="bi bi-bootstrap"></i></div>
                          <div class="col"><i class="fa-brands fa-vuejs"></i></div>
                          <div class="col"><i class="fa-brands fa-node-js"></i></div>
                          <div class="col"><i class="bi bi-filetype-sql"></i></div>
                        </div>
                  </div>
                  <div class="col-sm-6">
                    <b>Soft Skills</b>
                    <br><br>
                    <ul data-aos="fade-left" v-for="i in skills" :key="i">
                        <li>{{ i.skill }}</li>
                    </ul>
                  </div>
                </div>
            </div>
    </div>
</template>

<script>
export default {
    data() {
        return {
            resume : [
                {
                    institution: "Highschool",
                    description: "Graduated from South Peninsula High School 2021. Passed Matric with bachelors",
                    year: "2017- 2021",
                },
                {
                    institution: "IT Academy",
                    description: "Completed Software Fundamentals Course",
                    year: "March 2022 - March 2023"
                },
                {
                    institution: "Life Choice Academy",
                    description: "Completed FullStack Developer Course",
                    year: "September 2022 - March 2023"
                }
            ],
            skills : [
                {
                    skill: "Work Ethics Training"
                },
                {
                    skill: "Interview Training"
                },
                {
                    skill: "Professional/Personal Development"
                }
            ]
        }
    }
}
</script>

<style scoped>
#resume {
    background-image: linear-gradient(white, rgb(103, 172, 224));
    height: auto;
} 

p {
    font-size: large;
}

i {
    font-size: 50px;
  }

b {
    color:rgb(0, 44, 78);
	font-size: larger;
}
.container {
    justify-content: center;
    position: relative;
    display: block;
    margin: auto;
    padding: 50px;
    border: 1px solid white;
    border-radius: 5px;
    box-shadow: 0 20px 30px rgba(0,0,0,0.2);
    backdrop-filter: blur(10px); 
    transition: all 0.3s;
    transform: scale(1);
}
.timeline ul{
	list-style-type:none;
	border-left:2px solid rgb(0, 44, 78);
	padding:10px 5px;
}
.timeline ul li{
	padding:20px 20px;
	position:relative;
	cursor:pointer;
	transition:.5s;
}
.timeline ul li span{
	display:inline-block;
	background-color: transparent;
	border-radius:2px;
    border: 1px solid white;
	padding:2px 5px;
	font-size:15px;
	text-align:center;
}
.timeline ul li .content h3{
	color:rgb(0, 44, 78);
	font-size: larger;
	padding-top:5px;
}
.timeline ul li .content p{
	padding:5px 0px 15px 0px;
	font-size:15px;
}
.timeline ul li:before{
	position:absolute;
	content:'';
	width:10px;
	height:10px;
	background-color:white;
	border-radius:50%;
	left:-11px;
	top:70px;
	transition:.5s;
}
.timeline ul li:hover{
	background-color: rgb(103, 172, 224);
}
.timeline ul li:hover:before{
	background-color:rgb(0, 44, 78);
	box-shadow:0px 0px 10px 2px rgb(0, 44, 78);
}
@media (max-width:300px){
	.timeline{
		width:100%;
		padding:30px 5px 30px 10px;
	}
	.timeline ul li .content h3{
		color:rgb(103, 172, 224);
		font-size:15px;
	}

}

</style>
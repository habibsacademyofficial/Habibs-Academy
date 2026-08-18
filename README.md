# Habibs-Academy
Habib's Academy Official Website
<!DOCTYPE html>
<html lang="bn">
<head>
<meta charset="UTF-8">
<meta name="viewport" content="width=device-width, initial-scale=1.0">

<title>Habib's Academy | Business Studies</title>

<!-- Font Awesome -->
<link rel="stylesheet"
href="https://cdnjs.cloudflare.com/ajax/libs/font-awesome/6.5.2/css/all.min.css">

<!-- Google Fonts -->
<link rel="preconnect" href="https://fonts.googleapis.com">
<link rel="preconnect" href="https://fonts.gstatic.com" crossorigin>
<link href="https://fonts.googleapis.com/css2?family=Hind+Siliguri:wght@400;500;600;700&family=Poppins:wght@400;500;600;700&display=swap" rel="stylesheet">

<style>

:root{
    --blue:#0066cc;
    --teal:#00b4d8;
    --green:#70e000;
    --yellow:#ffb703;
    --orange:#fb8500;
    --pink:#e63946;

    --dark:#0f172a;
    --card:#1e293b;
    --text:#f8fafc;
    --muted:#94a3b8;

    --gradient:linear-gradient(
        135deg,
        #0066cc,
        #00b4d8,
        #70e000,
        #ffb703,
        #e63946
    );
}

*{
    margin:0;
    padding:0;
    box-sizing:border-box;
}

html{
    scroll-behavior:smooth;
}

body{
    background:var(--dark);
    color:var(--text);
    line-height:1.6;
    font-family:'Hind Siliguri','Poppins',sans-serif;
    overflow-x:hidden;
}

a{
    text-decoration:none;
}

button,
input,
textarea,
select{
    font-family:inherit;
}


/* ================= HEADER ================= */

header{
    position:fixed;
    top:0;
    left:0;
    width:100%;
    z-index:9999;

    background:rgba(15,23,42,.96);
    backdrop-filter:blur(12px);

    border-bottom:1px solid rgba(255,255,255,.08);
}

.navbar{
    max-width:1200px;
    margin:auto;

    min-height:75px;
    padding:12px 20px;

    display:flex;
    align-items:center;
    justify-content:space-between;

    gap:20px;
}

.logo-container{
    display:flex;
    align-items:center;
    gap:10px;
    color:white;
}

.logo-icon{
    display:flex;
    align-items:flex-end;
    gap:3px;
    height:36px;
}

.logo-bar{
    width:7px;
    border-radius:5px;
}

.bar-1{
    height:60%;
    background:#0066cc;
}

.bar-2{
    height:80%;
    background:#00b4d8;
}

.bar-3{
    height:100%;
    background:#70e000;
}

.bar-4{
    height:100%;
    background:#ffb703;
}

.bar-5{
    height:80%;
    background:#fb8500;
}

.bar-6{
    height:60%;
    background:#e63946;
}

.logo-text h1{
    font-family:Poppins,sans-serif;
    font-size:1.25rem;
    line-height:1.1;
}

.logo-text span{
    display:block;
    color:#ffb703;
    font-size:.55rem;
    letter-spacing:.4px;
}

.nav-links{
    display:flex;
    align-items:center;
    gap:20px;
    list-style:none;
}

.nav-links a{
    color:#f8fafc;
    font-size:.95rem;
    transition:.3s;
}

.nav-links a:hover{
    color:#ffb703;
}

.menu-toggle{
    display:none;
    font-size:1.6rem;
    cursor:pointer;
    color:white;
}


/* ================= BUTTON ================= */

.btn{
    display:inline-flex;
    align-items:center;
    justify-content:center;

    gap:8px;

    padding:10px 22px;

    border:none;
    border-radius:30px;

    font-weight:600;
    cursor:pointer;

    transition:.3s;
}

.btn:hover{
    transform:translateY(-3px);
}

.btn-primary{
    background:linear-gradient(45deg,#0066cc,#00b4d8);
    color:white;
    box-shadow:0 5px 20px rgba(0,180,216,.3);
}

.btn-secondary{
    background:linear-gradient(45deg,#fb8500,#ffb703);
    color:#111;
}

.btn-outline{
    border:1px solid #00b4d8;
    background:transparent;
    color:white;
}

.btn-outline:hover{
    background:#00b4d8;
}


/* ================= HERO ================= */

.hero{
    max-width:1200px;
    min-height:100vh;

    margin:auto;
    padding:150px 20px 80px;

    display:flex;
    align-items:center;
    gap:60px;
}

.hero-content{
    flex:1;
}

.hero-badge{
    display:inline-block;

    padding:7px 15px;
    margin-bottom:20px;

    border-radius:20px;

    background:rgba(255,183,3,.12);
    border:1px solid rgba(255,183,3,.3);

    color:#ffb703;
}

.hero h1{
    font-size:3rem;
    line-height:1.2;
    margin-bottom:20px;
}

.highlight-text{
    background:var(--gradient);
    background-clip:text;
    -webkit-background-clip:text;
    color:transparent;
}

.hero p{
    color:var(--muted);
    font-size:1.1rem;
    margin-bottom:30px;
}

.hero-buttons{
    display:flex;
    gap:15px;
    flex-wrap:wrap;
}

.hero-image{
    flex:1;
    display:flex;
    justify-content:center;
}

.main-card{
    width:320px;
    min-height:380px;

    padding:35px 25px;

    border-radius:25px;

    background:var(--card);

    border:1px solid rgba(255,255,255,.1);

    box-shadow:0 20px 50px rgba(0,0,0,.45);

    display:flex;
    flex-direction:column;
    justify-content:center;
    align-items:center;

    text-align:center;

    position:relative;
}

.main-card::before{
    content:"";

    position:absolute;
    inset:-2px;

    background:var(--gradient);

    border-radius:27px;

    z-index:-1;

    filter:blur(12px);

    opacity:.5;
}


/* ================= STATS ================= */

.stats-section{
    background:var(--card);
    padding:40px 20px;

    border-top:1px solid rgba(255,255,255,.05);
    border-bottom:1px solid rgba(255,255,255,.05);
}

.stats-container{
    max-width:1200px;
    margin:auto;

    display:grid;
    grid-template-columns:repeat(4,1fr);

    gap:25px;

    text-align:center;
}

.stat-item h2{
    color:#00b4d8;
    font-size:2.3rem;
}

.stat-item p{
    color:var(--muted);
}


/* ================= SECTION ================= */

.section{
    max-width:1200px;
    margin:auto;
    padding:90px 20px;
}

.section-title{
    text-align:center;
    margin-bottom:50px;
}

.section-title h2{
    font-size:2.2rem;
    margin-bottom:10px;
}

.section-title p{
    color:var(--muted);
}


/* ================= FEATURES ================= */

.features-grid{
    display:grid;
    grid-template-columns:repeat(4,1fr);
    gap:25px;
}

.feature-card{
    padding:30px;
    background:var(--card);
    border:1px solid rgba(255,255,255,.06);
    border-radius:18px;

    transition:.3s;
}

.feature-card:hover{
    transform:translateY(-7px);
    border-color:#00b4d8;
}

.feature-icon{
    width:60px;
    height:60px;

    display:flex;
    align-items:center;
    justify-content:center;

    border-radius:14px;

    font-size:1.5rem;

    margin-bottom:20px;
}

.feature-card p{
    color:var(--muted);
    margin-top:10px;
}


/* ================= COURSE FILTER ================= */

.course-filter{
    display:flex;
    justify-content:center;
    flex-wrap:wrap;

    gap:10px;

    margin-bottom:40px;
}

.filter-btn{
    padding:9px 20px;

    border-radius:25px;

    border:1px solid rgba(255,255,255,.1);

    background:var(--card);

    color:var(--muted);

    cursor:pointer;

    transition:.3s;
}

.filter-btn:hover,
.filter-btn.active{
    background:#00b4d8;
    color:white;
}


/* ================= COURSES ================= */

.courses-grid{
    display:grid;
    grid-template-columns:repeat(3,1fr);
    gap:25px;
}

.course-card{
    background:var(--card);
    border:1px solid rgba(255,255,255,.08);

    border-radius:20px;

    overflow:hidden;

    display:flex;
    flex-direction:column;

    transition:.3s;
}

.course-card:hover{
    transform:translateY(-7px);
    box-shadow:0 15px 35px rgba(0,0,0,.35);
}

.course-header{
    padding:25px;

    background:linear-gradient(
        135deg,
        rgba(0,102,204,.2),
        rgba(0,180,216,.1)
    );
}

.course-tag{
    display:inline-block;

    background:#e63946;

    padding:4px 10px;

    border-radius:15px;

    font-size:.75rem;

    margin-bottom:12px;
}

.course-header h3{
    margin-bottom:5px;
}

.course-header p{
    color:var(--muted);
    font-size:.9rem;
}

.course-body{
    padding:25px;

    display:flex;
    flex-direction:column;

    flex:1;
}

.course-features{
    list-style:none;
    margin-bottom:25px;
}

.course-features li{
    color:var(--muted);
    margin-bottom:10px;

    display:flex;
    gap:8px;
}

.course-features i{
    color:#70e000;
    margin-top:5px;
}

.course-footer{
    margin-top:auto;

    padding-top:18px;

    border-top:1px solid rgba(255,255,255,.06);

    display:flex;
    justify-content:space-between;
    align-items:center;

    gap:10px;
}

.price{
    color:#ffb703;
    font-size:1.3rem;
    font-weight:bold;
}


/* ================= INSTRUCTOR ================= */

.instructor-card{
    background:var(--card);
    border:1px solid rgba(255,255,255,.06);

    border-radius:18px;

    padding:30px;

    text-align:center;
}

.instructor-avatar{
    width:110px;
    height:110px;

    margin:0 auto 15px;

    padding:3px;

    border-radius:50%;

    background:var(--gradient);
}

.instructor-avatar img{
    width:100%;
    height:100%;

    border-radius:50%;

    object-fit:cover;

    background:var(--dark);
}


/* ================= TESTIMONIAL ================= */

.testimonials-grid{
    display:grid;
    grid-template-columns:repeat(3,1fr);
    gap:25px;
}

.testimonial-card{
    background:var(--card);

    border:1px solid rgba(255,255,255,.06);

    border-radius:18px;

    padding:25px;

    position:relative;
}

.quote{
    position:absolute;

    right:20px;
    top:20px;

    font-size:2rem;

    color:rgba(255,255,255,.1);
}

.testimonial-card > p{
    color:var(--muted);
}

.student-info{
    display:flex;
    align-items:center;

    gap:12px;

    margin-top:20px;
}

.student-avatar{
    width:45px;
    height:45px;

    border-radius:50%;

    display:flex;
    align-items:center;
    justify-content:center;

    background:#00b4d8;

    font-weight:bold;
}


/* ================= FAQ ================= */

.faq-container{
    max-width:800px;
    margin:auto;
}

.faq-item{
    background:var(--card);

    border:1px solid rgba(255,255,255,.06);

    border-radius:12px;

    margin-bottom:12px;

    overflow:hidden;
}

.faq-question{
    padding:20px;

    display:flex;
    justify-content:space-between;
    align-items:center;

    cursor:pointer;

    font-weight:600;
}

.faq-question i{
    transition:.3s;
}

.faq-answer{
    display:none;

    padding:0 20px 20px;

    color:var(--muted);
}

.faq-item.active .faq-answer{
    display:block;
}

.faq-item.active .faq-question i{
    transform:rotate(180deg);
    color:#00b4d8;
}


/* ================= CONTACT ================= */

.contact-box{
    background:var(--card);

    border:1px solid rgba(255,255,255,.08);

    border-radius:25px;

    padding:40px;

    display:grid;
    grid-template-columns:1fr 1fr;

    gap:40px;
}

.contact-info p{
    color:var(--muted);
    margin-bottom:25px;
}

.contact-line{
    display:flex;
    align-items:center;

    gap:15px;

    margin-bottom:18px;
}

.contact-line i{
    color:#00b4d8;
}

.form-group{
    margin-bottom:18px;
}

.form-group input,
.form-group textarea,
.form-group select{
    width:100%;

    padding:13px 16px;

    background:rgba(15,23,42,.8);

    color:white;

    border:1px solid rgba(255,255,255,.1);

    border-radius:10px;

    outline:none;
}

.form-group select option{
    background:#1e293b;
    color:white;
}

.form-group input:focus,
.form-group textarea:focus,
.form-group select:focus{
    border-color:#00b4d8;
}


/* ================= FOOTER ================= */

footer{
    background:#080d1a;

    padding:50px 20px 20px;

    border-top:1px solid rgba(255,255,255,.05);
}

.footer-content{
    max-width:1200px;

    margin:auto;

    display:grid;

    grid-template-columns:2fr 1fr 1fr;

    gap:40px;

    margin-bottom:40px;
}

.footer-content p,
.footer-content li{
    color:var(--muted);
}

.footer-content a{
    color:inherit;
}

.social-icons{
    margin-top:20px;
}

.social-icons a{
    font-size:1.3rem;
    margin-right:15px;
}

.footer-bottom{
    max-width:1200px;
    margin:auto;

    padding-top:20px;

    border-top:1px solid rgba(255,255,255,.05);

    text-align:center;

    color:var(--muted);

    font-size:.85rem;
}


/* ================= MOBILE ================= */

@media(max-width:900px){

    .nav-links{
        gap:12px;
    }

    .features-grid{
        grid-template-columns:repeat(2,1fr);
    }

    .courses-grid{
        grid-template-columns:repeat(2,1fr);
    }

    .testimonials-grid{
        grid-template-columns:1fr 1fr;
    }

}


@media(max-width:768px){

    .navbar{
        min-height:65px;
    }

    .logo-text h1{
        font-size:1rem;
    }

    .logo-text span{
        font-size:.45rem;
    }

    .navbar > .btn-primary{
        display:none;
    }

    .menu-toggle{
        display:block;
    }

    .nav-links{
        position:absolute;

        top:65px;
        left:0;

        width:100%;

        background:#1e293b;

        padding:20px;

        display:none;

        flex-direction:column;

        align-items:flex-start;

        gap:16px;

        border-top:1px solid rgba(255,255,255,.05);

        box-shadow:0 15px 30px rgba(0,0,0,.3);
    }

    .nav-links.active{
        display:flex;
    }

    .hero{
        flex-direction:column;

        text-align:center;

        padding-top:120px;

        gap:45px;
    }

    .hero h1{
        font-size:2.2rem;
    }

    .hero-buttons{
        justify-content:center;
    }

    .main-card{
        width:290px;
        min-height:350px;
    }

    .stats-container{
        grid-template-columns:repeat(2,1fr);
    }

    .features-grid{
        grid-template-columns:1fr;
    }

    .courses-grid{
        grid-template-columns:1fr;
    }

    .testimonials-grid{
        grid-template-columns:1fr;
    }

    .contact-box{
        grid-template-columns:1fr;
        padding:25px;
    }

    .footer-content{
        grid-template-columns:1fr;
    }

}


@media(max-width:450px){

    .hero{
        padding-left:15px;
        padding-right:15px;
    }

    .hero h1{
        font-size:1.9rem;
    }

    .hero p{
        font-size:1rem;
    }

    .hero-buttons .btn{
        width:100%;
    }

    .stats-container{
        grid-template-columns:1fr 1fr;
        gap:15px;
    }

    .stat-item h2{
        font-size:1.8rem;
    }

    .section{
        padding:65px 15px;
    }

    .section-title h2{
        font-size:1.8rem;
    }

    .course-footer{
        flex-direction:column;
        align-items:stretch;
    }

    .course-footer .btn{
        width:100%;
    }

}

</style>
</head>


<body>


<!-- ================= HEADER ================= -->

<header>

<div class="navbar">

<a href="#home" class="logo-container">

<div class="logo-icon">

<div class="logo-bar bar-1"></div>
<div class="logo-bar bar-2"></div>
<div class="logo-bar bar-3"></div>
<div class="logo-bar bar-4"></div>
<div class="logo-bar bar-5"></div>
<div class="logo-bar bar-6"></div>

</div>

<div class="logo-text">

<h1>Habib's Academy</h1>

<span>
A COMPLETE SOLUTION FOR BUSINESS STUDIES
</span>

</div>

</a>


<i class="fa-solid fa-bars menu-toggle" id="menuToggle"></i>


<ul class="nav-links" id="navLinks">

<li><a href="#home">Home</a></li>
<li><a href="#why-us">Why Us</a></li>
<li><a href="#courses">Courses</a></li>
<li><a href="#instructors">Instructors</a></li>
<li><a href="#testimonials">Reviews</a></li>
<li><a href="#faq">FAQ</a></li>
<li><a href="#contact">Contact</a></li>

</ul>


<a href="#courses" class="btn btn-primary">
Get Started
</a>

</div>

</header>



<!-- ================= HERO ================= -->

<section class="hero" id="home">

<div class="hero-content">

<span class="hero-badge">
<i class="fa-solid fa-graduation-cap"></i>
Best Business Studies Platform
</span>


<h1>

গড়ে তোলো তোমার

<br>

<span class="highlight-text">
বিজনেস স্টাডিজের
</span>

ভবিষ্যৎ

</h1>


<p>

HSC ও বিশ্ববিদ্যালয় ভর্তি পরীক্ষার সেরা প্রস্তুতি নাও
অভিজ্ঞ শিক্ষক ও প্রফেশনাল গাইডলাইনের মাধ্যমে।
কনসেপ্ট ক্লিয়ারিং থেকে মডেল টেস্ট—
সবকিছু একই ছাদের নিচে!

</p>


<div class="hero-buttons">

<a href="#courses" class="btn btn-primary">

<i class="fa-solid fa-book-open"></i>

Explore Courses

</a>


<a href="#contact" class="btn btn-secondary">

<i class="fa-solid fa-phone"></i>

Contact Us

</a>

</div>

</div>



<div class="hero-image">

<div class="main-card">

<div class="logo-icon" style="height:60px;">

<div class="logo-bar bar-1" style="width:12px;"></div>
<div class="logo-bar bar-2" style="width:12px;"></div>
<div class="logo-bar bar-3" style="width:12px;"></div>
<div class="logo-bar bar-4" style="width:12px;"></div>
<div class="logo-bar bar-5" style="width:12px;"></div>
<div class="logo-bar bar-6" style="width:12px;"></div>

</div>


<h2>HABIB'S ACADEMY</h2>

<p style="color:#ffb703;font-weight:bold;">
Learn • Grow • Succeed
</p>


<div style="
margin-top:20px;
padding:12px;
width:100%;
background:rgba(255,255,255,.05);
border-radius:10px;
">

<i class="fa-solid fa-check-circle"
style="color:#70e000;"></i>

100% Concept Clarity

</div>

</div>

</div>

</section>



<!-- ================= STATS ================= -->

<section class="stats-section">

<div class="stats-container">

<div class="stat-item">

<h2>১০০০+</h2>

<p>সফল শিক্ষার্থী</p>

</div>


<div class="stat-item">

<h2>৯৮%</h2>

<p>সাফল্য হার</p>

</div>


<div class="stat-item">

<h2>৫০+</h2>

<p>ফ্রি লেকচার ও নোটস</p>

</div>


<div class="stat-item">

<h2>২৪/৭</h2>

<p>ডাউট সলভিং সাপোর্ট</p>

</div>

</div>

</section>



<!-- ================= WHY US ================= -->

<section class="section" id="why-us">

<div class="section-title">

<h2>
কেন হাবিব'স একাডেমি?
</h2>

<p>
বিজনেস স্টাডিজ শিক্ষার্থীদের জন্য বিশেষ আয়োজন
</p>

</div>


<div class="features-grid">


<div class="feature-card">

<div class="feature-icon"
style="background:rgba(0,102,204,.15);color:#0066cc;">

<i class="fa-solid fa-chalkboard-user"></i>

</div>

<h3>লাইভ ইন্টারঅ্যাক্টিভ ক্লাস</h3>

<p>
লাইভ ক্লাস ও সরাসরি প্রশ্ন করার সুবিধা।
</p>

</div>



<div class="feature-card">

<div class="feature-icon"
style="background:rgba(112,224,0,.15);color:#70e000;">

<i class="fa-solid fa-calculator"></i>

</div>

<h3>হিসাববিজ্ঞান সহজের কৌশল</h3>

<p>
ডেবিট-ক্রেডিট ও জাবেদার সহজ টেকনিক।
</p>

</div>



<div class="feature-card">

<div class="feature-icon"
style="background:rgba(255,183,3,.15);color:#ffb703;">

<i class="fa-solid fa-vial-circle-check"></i>

</div>

<h3>নিয়মিত মডেল টেস্ট</h3>

<p>
অধ্যায়ভিত্তিক ও ফাইনাল মডেল টেস্ট।
</p>

</div>



<div class="feature-card">

<div class="feature-icon"
style="background:rgba(230,57,70,.15);color:#e63946;">

<i class="fa-solid fa-note-sticky"></i>

</div>

<h3>প্রিমিয়াম লেকচার শিট</h3>

<p>
সহজ ভাষায় তৈরি স্ট্যান্ডার্ড নোটস।
</p>

</div>


</div>

</section>



<!-- ================= COURSES ================= -->

<section class="section" id="courses">

<div class="section-title">

<h2>আমাদের কোর্সসমূহ</h2>

<p>
তোমার প্রয়োজন অনুযায়ী কোর্স বেছে নাও
</p>

</div>


<div class="course-filter">

<button class="filter-btn active" data-filter="all">
All Courses
</button>

<button class="filter-btn" data-filter="hsc">
HSC Academic
</button>

<button class="filter-btn" data-filter="admission">
Admission
</button>

<button class="filter-btn" data-filter="special">
Special Masterclass
</button>

</div>



<div class="courses-grid">


<!-- COURSE 1 -->

<div class="course-card" data-category="hsc">

<div class="course-header">

<span class="course-tag">
HSC 2025/2026
</span>

<h3>
HSC Business Studies Full Batch
</h3>

<p>
Accounting, Finance, Management & Marketing
</p>

</div>


<div class="course-body">

<ul class="course-features">

<li>
<i class="fa-solid fa-circle-check"></i>
সম্পূর্ণ সিলেবাস কভার
</li>

<li>
<i class="fa-solid fa-circle-check"></i>
৮০+ লাইভ ও রেকর্ডেড ক্লাস
</li>

<li>
<i class="fa-solid fa-circle-check"></i>
লেকচার শিট PDF
</li>

<li>
<i class="fa-solid fa-circle-check"></i>
১৫+ মডেল টেস্ট
</li>

</ul>


<div class="course-footer">

<span class="price">
৳ ৩,৫০০
</span>

<a href="#contact"
class="btn btn-outline enroll-btn"
data-course="HSC Business Studies Full Batch">

Enroll Now

</a>

</div>

</div>

</div>



<!-- COURSE 2 -->

<div class="course-card" data-category="admission">

<div class="course-header">

<span class="course-tag"
style="background:#fb8500;">

Admission

</span>

<h3>
Varsity 'C' Unit Admission Batch
</h3>

<p>
DU, RU, CU, GST & Other Public Varsities
</p>

</div>


<div class="course-body">

<ul class="course-features">

<li>
<i class="fa-solid fa-circle-check"></i>
বিশ্ববিদ্যালয় প্রশ্ন ব্যাংক
</li>

<li>
<i class="fa-solid fa-circle-check"></i>
শর্টকাট ট্রিক্স
</li>

<li>
<i class="fa-solid fa-circle-check"></i>
ডেইলি ও উইকলি এক্সাম
</li>

<li>
<i class="fa-solid fa-circle-check"></i>
স্পেশাল গাইডলাইন
</li>

</ul>


<div class="course-footer">

<span class="price">
৳ ৪,৫০০
</span>

<a href="#contact"
class="btn btn-outline enroll-btn"
data-course="Varsity C Unit Admission Batch">

Enroll Now

</a>

</div>

</div>

</div>



<!-- COURSE 3 -->

<div class="course-card" data-category="special">

<div class="course-header">

<span class="course-tag"
style="background:#70e000;color:#000;">

Special

</span>

<h3>
Accounting & Finance Masterclass
</h3>

<p>
হিসাববিজ্ঞান ও অর্থায়নের স্পেশাল ব্যাচ
</p>

</div>


<div class="course-body">

<ul class="course-features">

<li>
<i class="fa-solid fa-circle-check"></i>
Basic থেকে Advanced
</li>

<li>
<i class="fa-solid fa-circle-check"></i>
গাণিতিক সমস্যার সহজ সমাধান
</li>

<li>
<i class="fa-solid fa-circle-check"></i>
Doubt Clearing Session
</li>

<li>
<i class="fa-solid fa-circle-check"></i>
Practice Sheet
</li>

</ul>


<div class="course-footer">

<span class="price">
৳ ২,০০০
</span>

<a href="#contact"
class="btn btn-outline enroll-btn"
data-course="Accounting & Finance Masterclass">

Enroll Now

</a>

</div>

</div>

</div>


</div>

</section>



<!-- ================= INSTRUCTORS ================= -->

<section class="section" id="instructors">

<div class="section-title">

<h2>
শিক্ষকদের সাথে পরিচিত হও
</h2>

<p>
সঠিক দিকনির্দেশনার জন্য অভিজ্ঞ মেন্টর
</p>

</div>


<div class="courses-grid">


<div class="instructor-card">

<div class="instructor-avatar">

<img
src="https://images.unsplash.com/photo-1534528741775-53994a69daeb?auto=format&fit=crop&w=300&q=80"
alt="Instructor">

</div>

<h3>
Md. Habibullah
</h3>

<p style="color:#00b4d8;">
Founder & Lead Instructor
</p>

<p style="color:#94a3b8;">
Business Studies Specialist
</p>

</div>



<div class="instructor-card">

<div class="instructor-avatar">

<img
src="https://images.unsplash.com/photo-1507003211169-0a1dd7228f2d?auto=format&fit=crop&w=300&q=80"
alt="Instructor">

</div>

<h3>
Accounting Expert
</h3>

<p style="color:#00b4d8;">
Senior Instructor
</p>

<p style="color:#94a3b8;">
Management Specialist
</p>

</div>


</div>

</section>



<!-- ================= TESTIMONIALS ================= -->

<section class="section" id="testimonials">

<div class="section-title">

<h2>
শিক্ষার্থীদের মতামত
</h2>

<p>
আমাদের শিক্ষার্থীদের অভিজ্ঞতা
</p>

</div>


<div class="testimonials-grid">


<div class="testimonial-card">

<i class="fa-solid fa-quote-right quote"></i>

<p>
"হাবিব ভাইয়ের একাউন্টিং ক্লাসের পর জটিল জাবেদাগুলো অনেক সহজ হয়ে গেছে!"
</p>

<div class="student-info">

<div class="student-avatar">
R
</div>

<div>

<h4>
Rafiqul Islam
</h4>

<span style="color:#ffb703;font-size:.8rem;">
Dhaka College
</span>

</div>

</div>

</div>



<div class="testimonial-card">

<i class="fa-solid fa-quote-right quote"></i>

<p>
"Admission ব্যাচের শর্টকাট টেকনিক ও নিয়মিত পরীক্ষা আমাকে অনেক সাহায্য করেছে।"
</p>

<div class="student-info">

<div class="student-avatar"
style="background:#fb8500;">
S
</div>

<div>

<h4>
Sumi Akhter
</h4>

<span style="color:#ffb703;font-size:.8rem;">
DU Student
</span>

</div>

</div>

</div>



<div class="testimonial-card">

<i class="fa-solid fa-quote-right quote"></i>

<p>
"লেকচার শিটগুলো খুব সুন্দরভাবে সাজানো। পরীক্ষার আগে রিভিশনে অনেক কাজে লাগে।"
</p>

<div class="student-info">

<div class="student-avatar"
style="background:#e63946;">
T
</div>

<div>

<h4>
Tanvir Hossain
</h4>

<span style="color:#ffb703;font-size:.8rem;">
Rajshahi College
</span>

</div>

</div>

</div>


</div>

</section>



<!-- ================= FAQ ================= -->

<section class="section" id="faq">

<div class="section-title">

<h2>
সাধারণ কিছু প্রশ্ন
</h2>

<p>
Frequently Asked Questions
</p>

</div>


<div class="faq-container">


<div class="faq-item">

<div class="faq-question">

<span>
কোর্সগুলো কীভাবে পরিচালিত হয়?
</span>

<i class="fa-solid fa-chevron-down"></i>

</div>

<div class="faq-answer">

আমাদের ক্লাস অনলাইন প্ল্যাটফর্মের মাধ্যমে পরিচালিত হয়।
লাইভ ক্লাসের পাশাপাশি প্রয়োজন অনুযায়ী রেকর্ডেড ক্লাসও দেওয়া হবে।

</div>

</div>



<div class="faq-item">

<div class="faq-question">

<span>
ক্লাস মিস করলে কি পরে দেখা যাবে?
</span>

<i class="fa-solid fa-chevron-down"></i>

</div>

<div class="faq-answer">

হ্যাঁ। রেকর্ডেড ক্লাস থাকলে পরবর্তীতে সুবিধামতো দেখা যাবে।

</div>

</div>



<div class="faq-item">

<div class="faq-question">

<span>
পেমেন্ট কীভাবে করতে হবে?
</span>

<i class="fa-solid fa-chevron-down"></i>

</div>

<div class="faq-answer">

বিকাশ, নগদ বা রকেটের মাধ্যমে পেমেন্ট করা যাবে।
ভর্তির আগে আমাদের সাথে যোগাযোগ করে সঠিক পেমেন্ট নম্বর নিশ্চিত করে নেবে।

</div>

</div>


</div>

</section>



<!-- ================= CONTACT ================= -->

<section class="section" id="contact">

<div class="contact-box">


<div class="contact-info">

<h2>
যোগাযোগ বা এনরোল করতে মেসেজ দাও
</h2>

<p>
কোর্স সম্পর্কে জানতে বা ভর্তি হতে নিচের ফর্মটি পূরণ করো।
</p>


<div class="contact-line">

<i class="fa-solid fa-phone"></i>

<span>
+880 1700-000000
</span>

</div>


<div class="contact-line">

<i class="fa-solid fa-envelope"></i>

<span>
contact@habibsacademy.com
</span>

</div>


<div class="contact-line">

<i class="fa-solid fa-location-dot"></i>

<span>
Dhaka, Bangladesh
</span>

</div>

</div>



<form id="contactForm">


<div class="form-group">

<input
type="text"
id="studentName"
placeholder="তোমার নাম"
required>

</div>


<div class="form-group">

<input
type="tel"
id="studentPhone"
placeholder="মোবাইল নম্বর"
required>

</div>


<div class="form-group">

<select id="courseSelect" required>

<option value="" selected disabled>
কোন কোর্সে আগ্রহী?
</option>

<option value="HSC Business Studies Full Batch">
HSC Business Studies Full Batch
</option>

<option value="Varsity C Unit Admission Batch">
Varsity 'C' Unit Admission Batch
</option>

<option value="Accounting & Finance Masterclass">
Accounting & Finance Masterclass
</option>

</select>

</div>


<div class="form-group">

<textarea
id="studentMsg"
rows="4"
placeholder="তোমার প্রশ্ন বা মেসেজ">
</textarea>

</div>


<button
type="submit"
class="btn btn-primary"
style="width:100%;">

<i class="fa-solid fa-paper-plane"></i>

Submit Request

</button>

</form>

</div>

</section>



<!-- ================= FOOTER ================= -->

<footer>

<div class="footer-content">


<div>

<h3>
Habib's Academy
</h3>

<p style="margin-top:10px;">
A Complete Solution For Business Studies.
</p>


<div class="social-icons">

<a href="#" aria-label="Facebook">
<i class="fa-brands fa-facebook"></i>
</a>

<a href="#" aria-label="YouTube">
<i class="fa-brands fa-youtube"></i>
</a>

<a href="#" aria-label="Instagram">
<i class="fa-brands fa-instagram"></i>
</a>

</div>

</div>



<div>

<h4>
Quick Links
</h4>

<ul style="
list-style:none;
margin-top:15px;
">

<li>
<a href="#home">Home</a>
</li>

<li>
<a href="#courses">Courses</a>
</li>

<li>
<a href="#instructors">Instructors</a>
</li>

<li>
<a href="#contact">Contact</a>
</li>

</ul>

</div>



<div>

<h4>
Courses
</h4>

<ul style="
list-style:none;
margin-top:15px;
">

<li>HSC Accounting</li>
<li>HSC Finance</li>
<li>Business Management</li>
<li>Varsity Admission</li>

</ul>

</div>


</div>


<div class="footer-bottom">

© 2026 Habib's Academy.
All Rights Reserved.

</div>

</footer>



<!-- ================= JAVASCRIPT ================= -->

<script>

/* ================= MOBILE MENU ================= */

const menuToggle =
document.getElementById("menuToggle");

const navLinks =
document.getElementById("navLinks");


menuToggle.addEventListener("click", function(){

navLinks.classList.toggle("active");

});


/* Close mobile menu after clicking link */

document.querySelectorAll(".nav-links a")
.forEach(function(link){

link.addEventListener("click", function(){

navLinks.classList.remove("active");

});

});



/* ================= COURSE FILTER ================= */

const filterButtons =
document.querySelectorAll(".filter-btn");

const courseCards =
document.querySelectorAll(".course-card");


filterButtons.forEach(function(button){

button.addEventListener("click", function(){

const category =
this.getAttribute("data-filter");


/* Active button */

filterButtons.forEach(function(btn){

btn.classList.remove("active");

});

this.classList.add("active");


/* Filter cards */

courseCards.forEach(function(card){

const cardCategory =
card.getAttribute("data-category");


if(
category === "all" ||
cardCategory === category
){

card.style.display = "flex";

}else{

card.style.display = "none";

}

});

});

});



/* ================= ENROLL BUTTON ================= */

const enrollButtons =
document.querySelectorAll(".enroll-btn");


enrollButtons.forEach(function(button){

button.addEventListener("click", function(){

const selectedCourse =
this.getAttribute("data-course");


const courseSelect =
document.getElementById("courseSelect");


courseSelect.value =
selectedCourse;

});

});



/* ================= FAQ ================= */

const faqQuestions =
document.querySelectorAll(".faq-question");


faqQuestions.forEach(function(question){

question.addEventListener("click", function(){

const currentItem =
this.parentElement;


/* Optional: close other FAQ */

document.querySelectorAll(".faq-item")
.forEach(function(item){

if(item !== currentItem){

item.classList.remove("active");

}

});


currentItem.classList.toggle("active");

});

});



/* ================= CONTACT FORM ================= */

const contactForm =
document.getElementById("contactForm");


contactForm.addEventListener("submit", function(event){

event.preventDefault();


const name =
document.getElementById("studentName").value.trim();

const phone =
document.getElementById("studentPhone").value.trim();

const course =
document.getElementById("courseSelect").value;


if(!name || !phone || !course){

alert("দয়া করে প্রয়োজনীয় তথ্যগুলো পূরণ করুন।");

return;

}


alert(
"ধন্যবাদ " +
name +
"! আপনার রিকোয়েস্ট গ্রহণ করা হয়েছে।"
);


contactForm.reset();

});

</script>


</body>
</html>

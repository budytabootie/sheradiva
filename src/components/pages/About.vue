<template>
	<main :class="`${head}-page`" :id="link">
		<div class="head">
			<h1 class="hide">TENTANG KAMI</h1>
			<hr class="about hide">
		</div>
		<div class="body">
			<div class="columnAbout1 hide">
				<p>Lorem ipsum dolor sit amet, consectetur adipiscing elit, sed do eiusmod tempor incididunt ut labore et dolore magna aliqua.	</p>
				<p class="list"><doubleCheck />Ullamco laboris nisi ut aliquip ex ea commodo consequat</p>
				<p class="list"><doubleCheck />Ullamco laboris nisi ut aliquip ex ea commodo consequat</p>
				<p class="list"><doubleCheck />Ullamco laboris nisi ut aliquip ex ea commodo consequat</p>
			</div>
			<div class="columnAbout2 hide">
				<p>Ullamco laboris nisi ut aliquip ex ea commodo consequat. Duis aute irure dolor in reprehenderit in voluptate velit esse cillum dolore eu fugiat nulla pariatur. Excepteur sint occaecat cupidatat non proident, sunt in culpa qui officia deserunt mollit anim id est laborum.</p>
				<div class="btn-0">
					<a href="#"><span>Pelajari Selengkapnya</span></a>
				</div>
			</div>
		</div>
		<div class="body1 hide">
			<div class="wrap1">
				<div class="columnAbout3">
					<div class="child-head hide">
						<p>Impian Kami Dalam Membangun Sistem Bisnis Yang Dapat Di Pelajari Oleh Pemula Dengan Bimbingan Mentor Ahli</p>
					</div>
					<div class="child-list">
						<a href="#">
							<div class="list list1 hide"><span>01</span><p>Apa sih  Visi dari perusahaan kami?</p><i class="expand material-icons" :class="{ opened: expanded }">expand_more</i></div>
						</a>
						<a href="#">
							<div class="list list2 hide"><span>02</span><p>Bagaimana dengan misi kami?</p><i class="expand material-icons" :class="{ opened: expanded }">expand_more</i></div>
						</a>
						<a href="#">
							<div class="list list3 hide"><span>03</span><p>Kenapa harus memilih bisnis kami?</p><i class="expand material-icons" :class="{ opened: expanded }">expand_more</i></div>
						</a>
					</div>
				</div>
				<div class="columnAbout4 hide">
					<custDB />
				</div>
			</div>
			<div class="wrap2">
				<div class="columnAbout5 columnWrap2 hide">
						<svg width="28" height="27" viewBox="0 0 28 27" fill="none" xmlns="http://www.w3.org/2000/svg"><path d="M5.1975 1.3625C5.3618 1.17041 5.56577 1.01619 5.79536 0.910459C6.02495 0.804725 6.27473 0.749983 6.5275 0.75H21.4725C21.7253 0.749983 21.975 0.804725 22.2046 0.910459C22.4342 1.01619 22.6382 1.17041 22.8025 1.3625L27.3682 6.6895C27.7759 7.16521 28 7.77102 28 8.3975V8.84375C28.0001 9.70996 27.7296 10.5546 27.2262 11.2595C26.7228 11.9644 26.0118 12.4945 25.1924 12.7756C24.3731 13.0566 23.4864 13.0747 22.6563 12.8272C21.8262 12.5797 21.0942 12.0791 20.5625 11.3953C20.1742 11.8953 19.6767 12.3 19.108 12.5781C18.5392 12.8563 17.9144 13.0006 17.2812 13C16.6481 13.0007 16.0232 12.8565 15.4545 12.5783C14.8857 12.3001 14.3882 11.8954 14 11.3953C13.6118 11.8954 13.1143 12.3001 12.5455 12.5783C11.9768 12.8565 11.3519 13.0007 10.7188 13C10.0856 13.0007 9.46072 12.8565 8.89195 12.5783C8.32319 12.3001 7.82566 11.8954 7.4375 11.3953C6.90583 12.0791 6.17379 12.5797 5.34369 12.8272C4.51359 13.0747 3.6269 13.0566 2.80757 12.7756C1.98823 12.4945 1.27719 11.9644 0.773819 11.2595C0.270448 10.5546 -9.55475e-05 9.70996 2.53129e-08 8.84375V8.3975C2.20632e-05 7.77102 0.224099 7.16521 0.63175 6.6895L5.19925 1.36075L5.1975 1.3625ZM8.3125 8.84375C8.3125 9.48193 8.56601 10.094 9.01727 10.5452C9.46853 10.9965 10.0806 11.25 10.7188 11.25C11.3569 11.25 11.969 10.9965 12.4202 10.5452C12.8715 10.094 13.125 9.48193 13.125 8.84375C13.125 8.61169 13.2172 8.38913 13.3813 8.22503C13.5454 8.06094 13.7679 7.96875 14 7.96875C14.2321 7.96875 14.4546 8.06094 14.6187 8.22503C14.7828 8.38913 14.875 8.61169 14.875 8.84375C14.875 9.48193 15.1285 10.094 15.5798 10.5452C16.031 10.9965 16.6431 11.25 17.2812 11.25C17.9194 11.25 18.5315 10.9965 18.9827 10.5452C19.434 10.094 19.6875 9.48193 19.6875 8.84375C19.6875 8.61169 19.7797 8.38913 19.9438 8.22503C20.1079 8.06094 20.3304 7.96875 20.5625 7.96875C20.7946 7.96875 21.0171 8.06094 21.1812 8.22503C21.3453 8.38913 21.4375 8.61169 21.4375 8.84375C21.4375 9.48193 21.691 10.094 22.1423 10.5452C22.5935 10.9965 23.2056 11.25 23.8438 11.25C24.4819 11.25 25.094 10.9965 25.5452 10.5452C25.9965 10.094 26.25 9.48193 26.25 8.84375V8.3975C26.25 8.18895 26.1755 7.98725 26.04 7.82875L21.4725 2.5H6.5275L1.96 7.82875C1.82446 7.98725 1.74998 8.18895 1.75 8.3975V8.84375C1.75 9.48193 2.00352 10.094 2.45477 10.5452C2.90603 10.9965 3.51807 11.25 4.15625 11.25C4.79443 11.25 5.40647 10.9965 5.85773 10.5452C6.30899 10.094 6.5625 9.48193 6.5625 8.84375C6.5625 8.61169 6.65469 8.38913 6.81878 8.22503C6.98288 8.06094 7.20544 7.96875 7.4375 7.96875C7.66956 7.96875 7.89212 8.06094 8.05622 8.22503C8.22031 8.38913 8.3125 8.61169 8.3125 8.84375ZM2.625 13.875C2.85706 13.875 3.07962 13.9672 3.24372 14.1313C3.40781 14.2954 3.5 14.5179 3.5 14.75V25.25H5.25V16.5C5.25 16.0359 5.43437 15.5908 5.76256 15.2626C6.09075 14.9344 6.53587 14.75 7 14.75H12.25C12.7141 14.75 13.1592 14.9344 13.4874 15.2626C13.8156 15.5908 14 16.0359 14 16.5V25.25H24.5V14.75C24.5 14.5179 24.5922 14.2954 24.7563 14.1313C24.9204 13.9672 25.1429 13.875 25.375 13.875C25.6071 13.875 25.8296 13.9672 25.9937 14.1313C26.1578 14.2954 26.25 14.5179 26.25 14.75V25.25H27.125C27.3571 25.25 27.5796 25.3422 27.7437 25.5063C27.9078 25.6704 28 25.8929 28 26.125C28 26.3571 27.9078 26.5796 27.7437 26.7437C27.5796 26.9078 27.3571 27 27.125 27H0.875C0.642936 27 0.420376 26.9078 0.256282 26.7437C0.0921873 26.5796 2.53129e-08 26.3571 2.53129e-08 26.125C2.53129e-08 25.8929 0.0921873 25.6704 0.256282 25.5063C0.420376 25.3422 0.642936 25.25 0.875 25.25H1.75V14.75C1.75 14.5179 1.84219 14.2954 2.00628 14.1313C2.17038 13.9672 2.39294 13.875 2.625 13.875ZM7 25.25H12.25V16.5H7V25.25ZM15.75 16.5C15.75 16.0359 15.9344 15.5908 16.2626 15.2626C16.5908 14.9344 17.0359 14.75 17.5 14.75H21C21.4641 14.75 21.9092 14.9344 22.2374 15.2626C22.5656 15.5908 22.75 16.0359 22.75 16.5V21.75C22.75 22.2141 22.5656 22.6592 22.2374 22.9874C21.9092 23.3156 21.4641 23.5 21 23.5H17.5C17.0359 23.5 16.5908 23.3156 16.2626 22.9874C15.9344 22.6592 15.75 22.2141 15.75 21.75V16.5ZM21 16.5H17.5V21.75H21V16.5Z" fill="#47B2E4"/></svg>
					<h4>Modern Bisnis</h4><p>Memperkenalkan serta mengedukasi tentang apa itu bisnis era digital.</p>
				</div>
				<div class="columnAbout6 columnWrap2 hide">
					<svg width="28" height="28" viewBox="0 0 28 28" fill="none" xmlns="http://www.w3.org/2000/svg"><path d="M26.1485 21.9975L17.5 7.58625V1.75H18.375C18.8562 1.75 19.25 1.35625 19.25 0.875C19.25 0.39375 18.8562 0 18.375 0H9.625C9.14375 0 8.75 0.39375 8.75 0.875C8.75 1.35625 9.14375 1.75 9.625 1.75H10.5V7.58625L1.8515 21.9975C-0.129504 25.298 1.4 28 5.25 28H22.75C26.6 28 28.1295 25.2997 26.1485 21.9975ZM6.5905 17.5L12.25 8.0675V1.75H15.75V8.0675L21.4095 17.5H6.5905Z" fill="#47B2E4"/></svg>
					<h4>Uji Lab</h4><p>Produk yang sudah diuji kualitasnya melalui teknologi canggih labolatorium.</p>
				</div>
				<div class="columnAbout7 columnWrap2 hide">
					<svg width="26" height="20" viewBox="0 0 26 20" fill="none" xmlns="http://www.w3.org/2000/svg"><path d="M6.58334 19.3334C4.81389 19.3334 3.30228 18.7209 2.0485 17.4959C0.793949 16.2709 0.166672 14.7736 0.166672 13.0042C0.166672 11.4875 0.623616 10.1361 1.53751 8.95002C2.45139 7.76391 3.64723 7.00558 5.125 6.67502C5.61112 4.88613 6.58334 3.43752 8.04167 2.32919C9.5 1.22085 11.1528 0.666687 13 0.666687C15.275 0.666687 17.2047 1.45885 18.789 3.04319C20.3741 4.6283 21.1667 6.55835 21.1667 8.83335C22.5083 8.98891 23.6217 9.56719 24.5068 10.5682C25.3912 11.57 25.8333 12.7417 25.8333 14.0834C25.8333 15.5417 25.3231 16.7815 24.3027 17.8027C23.2814 18.8231 22.0417 19.3334 20.5833 19.3334H6.58334ZM11.075 15.3375C11.2306 15.3375 11.3764 15.313 11.5125 15.264C11.6486 15.2158 11.775 15.1334 11.8917 15.0167L16.8208 10.0875C17.0542 9.85419 17.1708 9.57224 17.1708 9.24169C17.1708 8.91113 17.0542 8.62919 16.8208 8.39585C16.5875 8.16252 16.3056 8.04585 15.975 8.04585C15.6444 8.04585 15.3625 8.16252 15.1292 8.39585L11.0458 12.4792L9.41251 10.8459C9.17917 10.6125 8.90695 10.4959 8.59584 10.4959C8.28473 10.4959 8.01251 10.6125 7.77917 10.8459C7.54584 11.0792 7.42917 11.3565 7.42917 11.6777C7.42917 11.9981 7.54584 12.275 7.77917 12.5084L10.2583 15.0167C10.375 15.1334 10.5014 15.2158 10.6375 15.264C10.7736 15.313 10.9194 15.3375 11.075 15.3375ZM6.58334 17H20.5833C21.4 17 22.0903 16.7181 22.6542 16.1542C23.2181 15.5903 23.5 14.9 23.5 14.0834C23.5 13.2667 23.2181 12.5764 22.6542 12.0125C22.0903 11.4486 21.4 11.1667 20.5833 11.1667H18.8333V8.83335C18.8333 7.21946 18.2648 5.84358 17.1277 4.70569C15.9898 3.56858 14.6139 3.00002 13 3.00002C11.3861 3.00002 10.0106 3.56858 8.87351 4.70569C7.73562 5.84358 7.16667 7.21946 7.16667 8.83335H6.58334C5.45556 8.83335 4.49306 9.23196 3.69584 10.0292C2.89862 10.8264 2.50001 11.7889 2.50001 12.9167C2.50001 14.0445 2.89862 15.007 3.69584 15.8042C4.49306 16.6014 5.45556 17 6.58334 17Z" fill="#47B2E4"/></svg>
					<h4>Trend Produk</h4><p>Dengan banyaknya permintaan pasar dan hasil riset sehingga mudah untuk dijual.</p>
				</div>
				<div class="columnAbout8 columnWrap2 hide">
					<svg width="20" height="24" viewBox="0 0 20 24" fill="none" xmlns="http://www.w3.org/2000/svg"><path d="M9.39557 0.605809L2.42796 3.21866C1.52217 3.56704 0.918312 4.42638 0.918312 5.40185V10.8714C0.918312 16.7358 4.87824 22.2054 10.2085 23.5409C15.5387 22.2054 19.4986 16.7358 19.4986 10.8714V5.40185C19.4978 4.92928 19.3528 4.46821 19.0831 4.08019C18.8133 3.69217 18.4316 3.39567 17.989 3.23027L11.0213 0.617421C10.4988 0.408393 9.91814 0.408393 9.39557 0.605809ZM8.15301 15.2029L5.69112 12.7411C5.58361 12.6335 5.49833 12.5059 5.44014 12.3654C5.38196 12.225 5.35201 12.0744 5.35201 11.9224C5.35201 11.7703 5.38196 11.6198 5.44014 11.4793C5.49833 11.3388 5.58361 11.2112 5.69112 11.1037C5.79864 10.9962 5.92627 10.9109 6.06674 10.8527C6.20721 10.7945 6.35777 10.7646 6.50982 10.7646C6.66186 10.7646 6.81242 10.7945 6.95289 10.8527C7.09336 10.9109 7.221 10.9962 7.32851 11.1037L8.9659 12.7411L13.0768 8.63017C13.1843 8.52266 13.3119 8.43738 13.4524 8.37919C13.5929 8.321 13.7434 8.29106 13.8955 8.29106C14.0475 8.29106 14.1981 8.321 14.3386 8.37919C14.479 8.43738 14.6067 8.52266 14.7142 8.63017C14.8217 8.73768 14.907 8.86532 14.9652 9.00579C15.0233 9.14626 15.0533 9.29682 15.0533 9.44886C15.0533 9.60091 15.0233 9.75147 14.9652 9.89194C14.907 10.0324 14.8217 10.16 14.7142 10.2676L9.7904 15.1913C9.34912 15.6558 8.60591 15.6558 8.15301 15.2029Z" fill="#47B2E4"/></svg>
					<h4>Keamanan Sistem</h4><p>Data yang ada dalam sistem akan secara otomatis terenkripsi sehingga tidak akan ada kebocoran data.</p>
				</div>
			</div>
			<div class="wrap3">
				<div class="onWrap">
					<div class="columnAbout9 columnWrap2 hide">
						<svg width="28" height="27" viewBox="0 0 28 27" fill="none" xmlns="http://www.w3.org/2000/svg"><path d="M5.1975 1.3625C5.3618 1.17041 5.56577 1.01619 5.79536 0.910459C6.02495 0.804725 6.27473 0.749983 6.5275 0.75H21.4725C21.7253 0.749983 21.975 0.804725 22.2046 0.910459C22.4342 1.01619 22.6382 1.17041 22.8025 1.3625L27.3682 6.6895C27.7759 7.16521 28 7.77102 28 8.3975V8.84375C28.0001 9.70996 27.7296 10.5546 27.2262 11.2595C26.7228 11.9644 26.0118 12.4945 25.1924 12.7756C24.3731 13.0566 23.4864 13.0747 22.6563 12.8272C21.8262 12.5797 21.0942 12.0791 20.5625 11.3953C20.1742 11.8953 19.6767 12.3 19.108 12.5781C18.5392 12.8563 17.9144 13.0006 17.2812 13C16.6481 13.0007 16.0232 12.8565 15.4545 12.5783C14.8857 12.3001 14.3882 11.8954 14 11.3953C13.6118 11.8954 13.1143 12.3001 12.5455 12.5783C11.9768 12.8565 11.3519 13.0007 10.7188 13C10.0856 13.0007 9.46072 12.8565 8.89195 12.5783C8.32319 12.3001 7.82566 11.8954 7.4375 11.3953C6.90583 12.0791 6.17379 12.5797 5.34369 12.8272C4.51359 13.0747 3.6269 13.0566 2.80757 12.7756C1.98823 12.4945 1.27719 11.9644 0.773819 11.2595C0.270448 10.5546 -9.55475e-05 9.70996 2.53129e-08 8.84375V8.3975C2.20632e-05 7.77102 0.224099 7.16521 0.63175 6.6895L5.19925 1.36075L5.1975 1.3625ZM8.3125 8.84375C8.3125 9.48193 8.56601 10.094 9.01727 10.5452C9.46853 10.9965 10.0806 11.25 10.7188 11.25C11.3569 11.25 11.969 10.9965 12.4202 10.5452C12.8715 10.094 13.125 9.48193 13.125 8.84375C13.125 8.61169 13.2172 8.38913 13.3813 8.22503C13.5454 8.06094 13.7679 7.96875 14 7.96875C14.2321 7.96875 14.4546 8.06094 14.6187 8.22503C14.7828 8.38913 14.875 8.61169 14.875 8.84375C14.875 9.48193 15.1285 10.094 15.5798 10.5452C16.031 10.9965 16.6431 11.25 17.2812 11.25C17.9194 11.25 18.5315 10.9965 18.9827 10.5452C19.434 10.094 19.6875 9.48193 19.6875 8.84375C19.6875 8.61169 19.7797 8.38913 19.9438 8.22503C20.1079 8.06094 20.3304 7.96875 20.5625 7.96875C20.7946 7.96875 21.0171 8.06094 21.1812 8.22503C21.3453 8.38913 21.4375 8.61169 21.4375 8.84375C21.4375 9.48193 21.691 10.094 22.1423 10.5452C22.5935 10.9965 23.2056 11.25 23.8438 11.25C24.4819 11.25 25.094 10.9965 25.5452 10.5452C25.9965 10.094 26.25 9.48193 26.25 8.84375V8.3975C26.25 8.18895 26.1755 7.98725 26.04 7.82875L21.4725 2.5H6.5275L1.96 7.82875C1.82446 7.98725 1.74998 8.18895 1.75 8.3975V8.84375C1.75 9.48193 2.00352 10.094 2.45477 10.5452C2.90603 10.9965 3.51807 11.25 4.15625 11.25C4.79443 11.25 5.40647 10.9965 5.85773 10.5452C6.30899 10.094 6.5625 9.48193 6.5625 8.84375C6.5625 8.61169 6.65469 8.38913 6.81878 8.22503C6.98288 8.06094 7.20544 7.96875 7.4375 7.96875C7.66956 7.96875 7.89212 8.06094 8.05622 8.22503C8.22031 8.38913 8.3125 8.61169 8.3125 8.84375ZM2.625 13.875C2.85706 13.875 3.07962 13.9672 3.24372 14.1313C3.40781 14.2954 3.5 14.5179 3.5 14.75V25.25H5.25V16.5C5.25 16.0359 5.43437 15.5908 5.76256 15.2626C6.09075 14.9344 6.53587 14.75 7 14.75H12.25C12.7141 14.75 13.1592 14.9344 13.4874 15.2626C13.8156 15.5908 14 16.0359 14 16.5V25.25H24.5V14.75C24.5 14.5179 24.5922 14.2954 24.7563 14.1313C24.9204 13.9672 25.1429 13.875 25.375 13.875C25.6071 13.875 25.8296 13.9672 25.9937 14.1313C26.1578 14.2954 26.25 14.5179 26.25 14.75V25.25H27.125C27.3571 25.25 27.5796 25.3422 27.7437 25.5063C27.9078 25.6704 28 25.8929 28 26.125C28 26.3571 27.9078 26.5796 27.7437 26.7437C27.5796 26.9078 27.3571 27 27.125 27H0.875C0.642936 27 0.420376 26.9078 0.256282 26.7437C0.0921873 26.5796 2.53129e-08 26.3571 2.53129e-08 26.125C2.53129e-08 25.8929 0.0921873 25.6704 0.256282 25.5063C0.420376 25.3422 0.642936 25.25 0.875 25.25H1.75V14.75C1.75 14.5179 1.84219 14.2954 2.00628 14.1313C2.17038 13.9672 2.39294 13.875 2.625 13.875ZM7 25.25H12.25V16.5H7V25.25ZM15.75 16.5C15.75 16.0359 15.9344 15.5908 16.2626 15.2626C16.5908 14.9344 17.0359 14.75 17.5 14.75H21C21.4641 14.75 21.9092 14.9344 22.2374 15.2626C22.5656 15.5908 22.75 16.0359 22.75 16.5V21.75C22.75 22.2141 22.5656 22.6592 22.2374 22.9874C21.9092 23.3156 21.4641 23.5 21 23.5H17.5C17.0359 23.5 16.5908 23.3156 16.2626 22.9874C15.9344 22.6592 15.75 22.2141 15.75 21.75V16.5ZM21 16.5H17.5V21.75H21V16.5Z" fill="#47B2E4"/></svg>
						<h4>Modern Bisnis</h4><p>Memperkenalkan serta mengedukasi tentang apa itu bisnis era digital.</p>
					</div>
					<div class="columnAbout10 columnWrap2 hide">
						<svg width="28" height="28" viewBox="0 0 28 28" fill="none" xmlns="http://www.w3.org/2000/svg"><path d="M26.1485 21.9975L17.5 7.58625V1.75H18.375C18.8562 1.75 19.25 1.35625 19.25 0.875C19.25 0.39375 18.8562 0 18.375 0H9.625C9.14375 0 8.75 0.39375 8.75 0.875C8.75 1.35625 9.14375 1.75 9.625 1.75H10.5V7.58625L1.8515 21.9975C-0.129504 25.298 1.4 28 5.25 28H22.75C26.6 28 28.1295 25.2997 26.1485 21.9975ZM6.5905 17.5L12.25 8.0675V1.75H15.75V8.0675L21.4095 17.5H6.5905Z" fill="#47B2E4"/></svg>
						<h4>Uji Lab</h4><p>Produk yang sudah diuji kualitasnya melalui teknologi canggih labolatorium.</p>
					</div>
				</div>
				<div class="onWrap">
					<div class="columnAbout11 columnWrap2 hide">
						<svg width="26" height="20" viewBox="0 0 26 20" fill="none" xmlns="http://www.w3.org/2000/svg"><path d="M6.58334 19.3334C4.81389 19.3334 3.30228 18.7209 2.0485 17.4959C0.793949 16.2709 0.166672 14.7736 0.166672 13.0042C0.166672 11.4875 0.623616 10.1361 1.53751 8.95002C2.45139 7.76391 3.64723 7.00558 5.125 6.67502C5.61112 4.88613 6.58334 3.43752 8.04167 2.32919C9.5 1.22085 11.1528 0.666687 13 0.666687C15.275 0.666687 17.2047 1.45885 18.789 3.04319C20.3741 4.6283 21.1667 6.55835 21.1667 8.83335C22.5083 8.98891 23.6217 9.56719 24.5068 10.5682C25.3912 11.57 25.8333 12.7417 25.8333 14.0834C25.8333 15.5417 25.3231 16.7815 24.3027 17.8027C23.2814 18.8231 22.0417 19.3334 20.5833 19.3334H6.58334ZM11.075 15.3375C11.2306 15.3375 11.3764 15.313 11.5125 15.264C11.6486 15.2158 11.775 15.1334 11.8917 15.0167L16.8208 10.0875C17.0542 9.85419 17.1708 9.57224 17.1708 9.24169C17.1708 8.91113 17.0542 8.62919 16.8208 8.39585C16.5875 8.16252 16.3056 8.04585 15.975 8.04585C15.6444 8.04585 15.3625 8.16252 15.1292 8.39585L11.0458 12.4792L9.41251 10.8459C9.17917 10.6125 8.90695 10.4959 8.59584 10.4959C8.28473 10.4959 8.01251 10.6125 7.77917 10.8459C7.54584 11.0792 7.42917 11.3565 7.42917 11.6777C7.42917 11.9981 7.54584 12.275 7.77917 12.5084L10.2583 15.0167C10.375 15.1334 10.5014 15.2158 10.6375 15.264C10.7736 15.313 10.9194 15.3375 11.075 15.3375ZM6.58334 17H20.5833C21.4 17 22.0903 16.7181 22.6542 16.1542C23.2181 15.5903 23.5 14.9 23.5 14.0834C23.5 13.2667 23.2181 12.5764 22.6542 12.0125C22.0903 11.4486 21.4 11.1667 20.5833 11.1667H18.8333V8.83335C18.8333 7.21946 18.2648 5.84358 17.1277 4.70569C15.9898 3.56858 14.6139 3.00002 13 3.00002C11.3861 3.00002 10.0106 3.56858 8.87351 4.70569C7.73562 5.84358 7.16667 7.21946 7.16667 8.83335H6.58334C5.45556 8.83335 4.49306 9.23196 3.69584 10.0292C2.89862 10.8264 2.50001 11.7889 2.50001 12.9167C2.50001 14.0445 2.89862 15.007 3.69584 15.8042C4.49306 16.6014 5.45556 17 6.58334 17Z" fill="#47B2E4"/></svg>
						<h4>Trend Produk</h4><p>Dengan banyaknya permintaan pasar dan hasil riset sehingga mudah untuk dijual.</p>
					</div>
					<div class="columnAbout12 columnWrap2 hide">
						<svg width="20" height="24" viewBox="0 0 20 24" fill="none" xmlns="http://www.w3.org/2000/svg"><path d="M9.39557 0.605809L2.42796 3.21866C1.52217 3.56704 0.918312 4.42638 0.918312 5.40185V10.8714C0.918312 16.7358 4.87824 22.2054 10.2085 23.5409C15.5387 22.2054 19.4986 16.7358 19.4986 10.8714V5.40185C19.4978 4.92928 19.3528 4.46821 19.0831 4.08019C18.8133 3.69217 18.4316 3.39567 17.989 3.23027L11.0213 0.617421C10.4988 0.408393 9.91814 0.408393 9.39557 0.605809ZM8.15301 15.2029L5.69112 12.7411C5.58361 12.6335 5.49833 12.5059 5.44014 12.3654C5.38196 12.225 5.35201 12.0744 5.35201 11.9224C5.35201 11.7703 5.38196 11.6198 5.44014 11.4793C5.49833 11.3388 5.58361 11.2112 5.69112 11.1037C5.79864 10.9962 5.92627 10.9109 6.06674 10.8527C6.20721 10.7945 6.35777 10.7646 6.50982 10.7646C6.66186 10.7646 6.81242 10.7945 6.95289 10.8527C7.09336 10.9109 7.221 10.9962 7.32851 11.1037L8.9659 12.7411L13.0768 8.63017C13.1843 8.52266 13.3119 8.43738 13.4524 8.37919C13.5929 8.321 13.7434 8.29106 13.8955 8.29106C14.0475 8.29106 14.1981 8.321 14.3386 8.37919C14.479 8.43738 14.6067 8.52266 14.7142 8.63017C14.8217 8.73768 14.907 8.86532 14.9652 9.00579C15.0233 9.14626 15.0533 9.29682 15.0533 9.44886C15.0533 9.60091 15.0233 9.75147 14.9652 9.89194C14.907 10.0324 14.8217 10.16 14.7142 10.2676L9.7904 15.1913C9.34912 15.6558 8.60591 15.6558 8.15301 15.2029Z" fill="#47B2E4"/></svg>
						<h4>Keamanan Sistem</h4><p>Data yang ada dalam sistem akan secara otomatis terenkripsi sehingga tidak akan ada kebocoran data.</p>
					</div>
				</div>
			</div>
		</div>
	</main>
</template>

<script setup>
import { ref, onMounted } from 'vue'
import doubleCheck from '../../assets/doubleCheck.vue'
import custDB from '../../assets/custDB.vue'

let mainTag = "";

const props = defineProps({
	data: {
		type: Array
	},
	head: {
		type: String
	},
	link: {
		type: String
	}
})

onMounted(() =>{
	const eventScroll = document.getElementsByTagName("main")[0];

	const eventScroll1 = document.getElementsByClassName('button')

	eventScroll.addEventListener('wheel',(e) => {

		let deltaY = e.deltaY
		let classTag = document.querySelector('#' + props.link + ' h1')
		showTheSection(e,classTag,deltaY)
		classTag = document.querySelector('#' + props.link + ' hr')
		showTheSection(e,classTag,deltaY)
		classTag = document.querySelector('.columnAbout1')
		showTheSection(e,classTag,deltaY)
		classTag = document.querySelector('.columnAbout2')
		showTheSection(e,classTag,deltaY)
		classTag = document.querySelector('.child-head')
		showTheSection(e,classTag,deltaY)
		classTag = document.querySelector('.list1')
		showTheSection(e,classTag,deltaY)
		classTag = document.querySelector('.list2')
		showTheSection(e,classTag,deltaY)
		classTag = document.querySelector('.list3')
		showTheSection(e,classTag,deltaY)
		classTag = document.querySelector('.columnAbout4')
		showTheSection(e,classTag,deltaY)
		classTag = document.querySelector('.columnAbout5')
		showTheSection(e,classTag,deltaY)
		classTag = document.querySelector('.columnAbout6')
		showTheSection(e,classTag,deltaY)
		classTag = document.querySelector('.columnAbout7')
		showTheSection(e,classTag,deltaY)
		classTag = document.querySelector('.columnAbout8')
		showTheSection(e,classTag,deltaY)
		classTag = document.querySelector('.columnAbout9')
		showTheSection(e,classTag,deltaY)
		classTag = document.querySelector('.columnAbout10')
		showTheSection(e,classTag,deltaY)
		classTag = document.querySelector('.columnAbout11')
		showTheSection(e,classTag,deltaY)
		classTag = document.querySelector('.columnAbout12')
		showTheSection(e,classTag,deltaY)

	});

	[].slice.call(eventScroll1).forEach(item => {
		item.addEventListener('click',(e) => {

		let deltaY = document.querySelector('.button')
		let classTag = document.querySelector('#' + props.link + ' h1')
		showTheSection(e,topOfSection,item,classTag,deltaY)
		classTag = document.querySelector('#' + props.link + ' hr')
		showTheSection(e,topOfSection,item,classTag,deltaY)
		classTag = document.querySelector('.columnAbout1')
		showTheSection(e,topOfSection,item,classTag,deltaY)
		classTag = document.querySelector('.columnAbout2')
		showTheSection(e,topOfSection,item,classTag,deltaY)

		})
	})

	eventScroll.addEventListener('touchstart', (e) => {
		// Cache the client X/Y coordinates
		let clientPhoneX = e.touches[0].clientX;
		let clientPhoneY = e.touches[0].clientY;
		console.log(clientPhoneY);

		eventScroll.addEventListener('touchend', (e) => {
			clientPhoneX = e.changedTouches[0].clientX - clientPhoneX;
			clientPhoneY = e.changedTouches[0].clientY - clientPhoneY;
			console.log(clientPhoneY);

			let deltaY = clientPhoneY
			let classTag = document.querySelector('#' + props.link + ' h1')
			showTheSection(e,classTag,deltaY)
			classTag = document.querySelector('#' + props.link + ' hr')
			showTheSection(e,classTag,deltaY)
			classTag = document.querySelector('.columnAbout1')
			showTheSection(e,classTag,deltaY)
			classTag = document.querySelector('.columnAbout2')
			showTheSection(e,classTag,deltaY)
			classTag = document.querySelector('.child-head')
			showTheSection(e,classTag,deltaY)
			classTag = document.querySelector('.list1')
			showTheSection(e,classTag,deltaY)
			classTag = document.querySelector('.list2')
			showTheSection(e,classTag,deltaY)
			classTag = document.querySelector('.list3')
			showTheSection(e,classTag,deltaY)
			classTag = document.querySelector('.columnAbout4')
			showTheSection(e,classTag,deltaY)
			classTag = document.querySelector('.columnAbout5')
			showTheSection(e,classTag,deltaY)
			classTag = document.querySelector('.columnAbout6')
			showTheSection(e,classTag,deltaY)
			classTag = document.querySelector('.columnAbout7')
			showTheSection(e,classTag,deltaY)
			classTag = document.querySelector('.columnAbout8')
			showTheSection(e,classTag,deltaY)
			classTag = document.querySelector('.columnAbout9')
			showTheSection(e,classTag,deltaY)
			classTag = document.querySelector('.columnAbout10')
			showTheSection(e,classTag,deltaY)
			classTag = document.querySelector('.columnAbout11')
			showTheSection(e,classTag,deltaY)
			classTag = document.querySelector('.columnAbout12')
			showTheSection(e,classTag,deltaY)

			

		})

	}, false);

})
</script>

<style lang="scss" scoped>
@import url('https://fonts.googleapis.com/css2?family=Inter:wght@200;400;500;700&display=swap');

main {

	div {
		font-family: 'Inter', sans-serif;
		&.head {

			width: 100%;
			height: auto;
			height: 35px;
			display: block;
  			justify-content: center;

			h1 {
				color: #37517E;
				width: 185px;
				height: 29px;
				margin-left: auto;
				margin-right: auto;
				text-align: center;
				font-family: 'Inter', sans-serif;
				font-size: 24px;
				font-weight: 700;
				text-transform: uppercase;
				transition: 1.5s ease-out;

				&.hide {
					transform: translateY(-50px);
					opacity: 0;
				}

				&.show {
					transform: translateY(0px);
					opacity: 1;
				}
			}

			hr {
				&.about {
					width: 136px;
					padding-top: 7px;
					margin-left: auto;
					margin-right: auto;
					text-align: center;
					border: solid transparent 1px;
					border-top: solid #47B2E4 2px;
					transition: 1s ease-out;
					
				}
				&.hide {
					transform: translateX(50px);
					opacity: 0;
				}

				&.show {
					transform: translateX(0px);
					opacity: 1;
				}
			}
		}

		&.body {
			width: 100%;
			height: 100%;
			display: flex;
  			justify-content: center;
			padding: 0 10px;
			padding-top: 37px;
			font-family: 'Inter', sans-serif;
			font-weight: 400;
			font-size: 15px;
			transition: all 1s;

			div {
				margin-left: auto;
				margin-right: auto;
				transition: all 1.5s;

				&.columnAbout1 {
					width: 50%;
					justify-content: center;
					text-align: left;
					margin-right: 25px;
					
					p {
						width: auto;
						align-content: left;

						svg {
							margin-right: 15px;
						}

						&.list {
							padding-top: 13px;
						}
					}

					&.hide {
						transform: translateY(80px);
						opacity: 0;
					}

					&.show {
						transform: translateY(0px);
						opacity: 1;
					}
				}

				&.columnAbout2 {
					width: 50%;
					justify-content: center;
					text-align: left;
					padding-left: 25px;
					position: relative;

					.btn-0 {
						border: solid #47B2E4 1px;
						border-radius: 5px;
						padding: 10px 26px;
						position: absolute;
						bottom: 0;

						a{
							text-decoration: none;
							color: #47B2E4;
							font-size: 15px;
							font-weight: 500;
						}
					}

					&.hide {
						transform: translateY(-80px);
						opacity: 0;
					}

					&.show {
						transform: translateY(0px);
						opacity: 1;
					}
				}

			}
			
		}

		&.body1 {
			width: 100%;
			height: 100%;
			margin-top: 37px;
			background-color: #F3F5FA;
			position: relative;

			.wrap1 {
				width: 100%;
				height: 68%;
				display: flex;
				padding-left: 117px;
				
				.columnAbout3 {
					width: 100%;
					padding-top: 151px;

					.child-head {
						font-weight: 400;
						font-size: 20px;
						transition: all 3s;
						
						&.hide {
							transform: translateY(-170px);
							opacity: 0;
						}
						&.show {
							transform: translateX(-0px);
							opacity: 1;
						}

					}
					.child-list {
						
						a {
							text-decoration: none;

							.list {
								display: flex;
								padding: 15px 22px;
								margin-top: 14px;
								background-color: #fff;
								position: relative;
								border-radius: 4px;
								transition: all 3s;

								&.list1 {
									margin-top: 33px;

									&.hide {
										transform: translateX(-36px);
										opacity: 0;
									}
									&.show {
										transform: translateX(-0px);
										opacity: 1;
									}
								}
								&.list2 {
									
									&.hide {
										transform: translateX(-74px);
										opacity: 0;
									}
									&.show {
										transform: translateX(-0px);
										opacity: 1;
									}
								}
								&.list3 {
									
									&.hide {
										transform: translateX(-110px);
										opacity: 0;
									}
									&.show {
										transform: translateX(-0px);
										opacity: 1;
									}
								}

								span {
									padding-right: 18px;
									color: #47B2E4;
									font-weight: 600;
								}

								p {
									font-weight: 500;
									color: black;
								}

								i {
									width: 9.33px;
									position: absolute;
									right: 0;
									margin-right: 22px;

								}
							}
						}
					}
				}

				.columnAbout4 {
					width: 100%;
					transition: all 2s ease-out;
					
					&.hide {
						transform: translateY(140px);
						opacity: 0;
					}
					&.show {
						transform: translateY(133px);
						opacity: 1;
					}
					
					svg {
						width: 510px !important;
						height: 467px !important;
						position: absolute;
						right: 0;
						top: 0;
						margin-top: 0px;
					}
				}
			}

			.wrap3 {display: none;}
			.wrap2 {
				width: 100%;
				height: 32%;
				justify-content: center;
				padding-top: 133px;
				padding-bottom: 79px;
				align-content: center;
				display: flex;
				
				.columnWrap2 {
					width: 236px;
					background-color: white;
					margin-right: 16px;
					margin-left: 16px;
					margin-top: 8px;
					margin-bottom: 8px;
					border-radius: 4px;
					transition: all 2s ease-out;
					
					svg {
						margin: 27px 0 9px 20px;
						width: 26px;
						height: 28px;
					}

					h4 {
	
						margin: 0 0 0px 20px;
						font-weight: 500;
						font-size: 14px;
					}
					
					p {
						padding: 0 20px 26px 20px;
						bottom: 0;
						font-weight: 400;
						font-size: 10px;
						margin-top: 7px;
					}

					&.columnAbout5 {
						&.hide {
							transform: translateY(100px);
							opacity: 0;
						}
						&.show {
							transform: translateY(0px);
							opacity: 1;
						}
					}
					&.columnAbout6 {
						&.hide {
							transform: translateY(-100px);
							opacity: 0;
						}
						&.show {
							transform: translateY(0px);
							opacity: 1;
						}
					}
					&.columnAbout7 {
						&.hide {
							transform: translateY(100px);
							opacity: 0;
						}
						&.show {
							transform: translateY(0px);
							opacity: 1;
						}
					}
					&.columnAbout8 {
						&.hide {
							transform: translateY(-100px);
							opacity: 0;
						}
						&.show {
							transform: translateY(0px);
							opacity: 1;
						}
					}
				}
				
			}
		}

		@media screen and (max-width: 768px) {

			&.head {
				h1 {
					margin: 0 !important;
				}

					&.show {
						transform: translateX(0);
						opacity: 1;
					}
				}

				hr {

					margin-left: 24.5px !important;
				}
			}
			&.body {
				display: block;

				div {
					&.columnAbout1 {
						width: 100% !important;
						margin-left: 0;
						padding: -25px;

				}
				.columnAbout2 {
					width: 100% !important;
					margin-left: 0;
					padding-left: 0 !important;
					padding-top: 26px;

					p{
						padding-bottom: 73px;
					}
				}
			}

						&.hide {
							transform: translateX(100px);
							opacity: 0;
						}

						&.show {
							transform: translateX(0px);
							opacity: 1;
						}
					}
				}
			}

			&.body1 {
				
				.wrap1 {
					padding-top: 151px;
					flex-direction: column;
					align-items: center;
					padding-left: 0;
					padding: 20px;
					transform: rotate(180deg);

					.columnAbout3 {
						transform: rotate(180deg);
						padding-top: 20px;
					}
					
					.columnAbout4 {
						
						svg {
							transform: rotate(180deg);
							position: relative;
							margin-top: 20px;
							max-width: 480px !important;
							height: 267px !important;
						}

						&.show {
							transform: translateX(0);
						}
					}

				}
				.wrap2 {display: none;}
				.wrap3 {
					width: 100%;
					height: 32%;
					padding-top: 10px;
					padding-bottom: 10px;
					display: flex;
					flex-direction: column;
					justify-content: center;
					align-content: center;
					align-items: center;
					padding-top: 20px;
				}
			}
		}
			
	}
}
</style>

<script>
function showTheSection (e,mainTag,deltaY) {

		const topOfSection = mainTag.getBoundingClientRect().top;
		const userWindow = window.innerHeight;
		const currTar = topOfSection - userWindow + 20;
		console.log( topOfSection + "|" + userWindow + "|" + deltaY);
		if ( currTar > 0 - 80 && deltaY < -2) {

			mainTag.classList.remove('show')

		} else if ( currTar < 0 && deltaY >= 2 ) {

			mainTag.classList.add('show')
			

		}
		console.log(currTar);

		if (e.pointerId != undefined) {
			const recognizeIdButton = userWindow.getAttribute('id')
			const recognizeIdPage = deltaY.getAttribute('id')
			if (recognizeIdPage == recognizeIdButton) {
				mainTag.classList.remove('show')
				mainTag.classList.add('show')
			} else {
				mainTag.classList.remove('show')
			}
		}
	}
</script>
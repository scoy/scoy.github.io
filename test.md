---
title: scoy
subtitle: testing... 1
layout: page
show_sidebar: false
---

<body>
    <div class="container showGrid">
        <div id="outerHeader" class="span-24">
            <br />
        </div>
        <div id="pageContainer" class="span-24 relative" >            
            <div id="header" class="span-24">
                <div id="topBanner" class="span-24">
                    <img src="/content/images/top_950.png" />             
                </div>
                <div class="right">
                    <iframe id="authWidget" src="/authwidget" frameborder="0" scrolling="no"></iframe>
                </div>
                <div id="bannerMessage">
                    <h3 class="tight">Build Games. Play Games. Share Games.</h3>
                </div>
                <a id="getKoduButton" class="greenControl" href="http://www.microsoft.com/en-us/download/details.aspx?id=10056">Get Kodu</a>
            </div>            
            <form id="searchBox" class="input right" action="/search">
                <input id="searchInput" data-watermark="Search worlds..." class="watermarked left span-4 first" name="query" type="text" />
                <input id="searchGo" class="left span-1 last" type="submit" value="" />
            </form>
            <div id="menuBar" class="span-23 push-1 clear">
                        <a class="menuItem" href="http://www.kodugamelab.com/">Home</a>
                        <a class="menuItem selected" href="http://www.kodugamelab.com/worlds/">Worlds</a>
                        <a class="menuItem" href="http://www.kodugamelab.com/blog/">Blog</a>
                        <a class="menuItem" href="http://www.kodugamelab.com/faq/">FAQ</a>
                        <a class="menuItem" href="http://www.kodugamelab.com/tips/">Tips</a>
                        <a class="menuItem" href="http://www.kodugamelab.com/resources/">Resources</a>
                        <a class="menuItem" href="http://www.kodugamelab.com/about/">About</a>
            </div>
            <div id="main" class="span-22 push-1 first last">
                



    <div class="fall-2 span-22"></div>



<div id="newestGallery" class="span-21">
    <div class="span-21 first last">
        <h3 class="left span-20 tight wrap-1">Newest</h3>
            <a class="link right last" href="/browse/newest">See All</a>
        <div class="span-21 fall-1"></div>
    </div>
</div>

    <div class="fall-2 span-22"></div>



<div id="popularGallery" class="span-21">
    <div class="span-21 first last">
        <h3 class="left span-20 tight wrap-1">Most Downloaded</h3>
            <a class="link right last" href="/browse/popular">See All</a>
        <div class="span-21 fall-1"></div>
    </div>
</div>

    <div class="fall-2 span-22"></div>



<div id="highestRatedGallery" class="span-21">
    <div class="span-21 first last">
        <h3 class="left span-21 tight wrap-1">Most Liked on Socl</h3>
        <div class="span-21 fall-1"></div>
    </div>
</div>


            </div>
            <div id="footer" class="span-24">
            </div>
        </div>
        <div id="outerFooter" class="span-24">
            <div class="span-24 fall-1"></div>
            <div class="left">
                <a href="http://research.microsoft.com">
                    <img class="left" src="/Content/Images/logo_msr.png"/>
                </a>
                <a href="http://fuse.microsoft.com">
                    <img class="left push-1" src="/Content/Images/logo_fuse.png" />
                </a>
            </div>
            <div class="right large-2">
                <a href="/Link/TermsOfUse">Terms of Use</a>
                <span> | </span>
                <a href="/Link/PrivacyStatement">Privacy Statement</a>
                <span> | </span>
                <a href="mailto:kodusupport@microsoft.com">Contact Us</a>
            </div>
            <div class="span-24 fall-2"></div>
        </div>
    </div>
    <div id="fb-root">
    </div>
    
    
    <script id="MessageTmpl" type="text/x-jquery-tmpl"><div id="${id}" class="${type}">
    ${text} - <a onclick="javascript:$(this).parent().remove();">Remove</a>
</div></script>
    <script id="RatingTmpl" type="text/x-jquery-tmpl">
<div class="rating span-3 ${voteable ? 'voteable' : ''}" >
    <div class="starsHolder" data-rating="${rating}" title="${rating} stars">
        <div class="star left-${rating > 0 ? 'full' : 'empty'}" data-starNum="1"></div>
        <div class="star right-${rating > 0.5 ? 'full' : 'empty'}" data-starNum="2"></div>
        <div class="star left-${rating > 1 ? 'full' : 'empty'}" data-starNum="3"></div>
        <div class="star right-${rating > 1.5 ? 'full' : 'empty'}" data-starNum="4"></div>
        <div class="star left-${rating > 2 ? 'full' : 'empty'}" data-starNum="5"></div>
        <div class="star right-${rating > 2.5 ? 'full' : 'empty'}" data-starNum="6"></div>
        <div class="star left-${rating > 3 ? 'full' : 'empty'}" data-starNum="7"></div>
        <div class="star right-${rating > 3.5 ? 'full' : 'empty'}" data-starNum="8"></div>
        <div class="star left-${rating > 4 ? 'full' : 'empty'}" data-starNum="9"></div>
        <div class="star right-${rating > 4.5 ? 'full' : 'empty'}" data-starNum="10"></div>
    </div>
    <span class="ratingCount ${ratingCount >= 1000 ? 'bold' : 'quiet'}" title="${ratingCount} ratings">(${KoduWeb.getSmallifiedNumber(ratingCount)})</span>
</div></script>
    

    <script src="https://ajax.aspnetcdn.com/ajax/jQuery/jquery-1.5.2.min.js" type="text/javascript"></script>
    <script src="https://ajax.aspnetcdn.com/ajax/jquery.templates/beta1/jquery.tmpl.min.js" type="text/javascript"></script>
    <script src="https://connect.facebook.net/en_US/all.js" type="text/javascript"></script>
    <script src="https://platform.twitter.com/widgets.js" type="text/javascript"></script>
    <script src="/Content/scripts/Master.js" type="text/javascript"></script>

    <script type="text/javascript">
        KoduWeb.fbAppId = 0;//SecurityManager.FacebookAppId;
        KoduWeb.userName = '';
        KoduWeb.userId = 0;
        KoduWeb.loggedIn = false;
    </script>
    
    



<script id="newestGalleryitemTmpl" type="text/x-jquery-tmpl">


<div class="galleryItem span-3 relative"
    data-itemNum="${GalleryItemNum}"
    >

    <div class="highlight"></div>

    <a class="worldThumbnail gallery block layer-1" href="/world/${World}">
        <img src="/API/Thumbnail?world=${World}" class=""/>
    </a>
    <a class="wrap-1 span-3 layer-1 world-name" href="/world/${World}">${Name}</a>
        <div class="span-3 layer-1 world-creator">
            <div class="left" style="width:15%">by </div>
            <span class="wrap-1 right quiet" style="width:84%" >${Creator}</span>
        </div>
        <div class="quiet wrap-1 span-3 layer-1 age">${Age}</div>
    <div class="fall-1 span-3"></div>

</div></script>

<script type="text/javascript">
    ///<reference path="Master.js" />

    KoduWeb['newestGallery'] = {
        galleryItemTmpl: $("#newestGalleryitemTmpl"),
        gallery: $("#" + "newestGallery"),
        hasPagination: false,
        worlds: [],

        init: function () {
            if (KoduWeb['newestGallery'].hasPagination)
            {
                var onPageChanged = KoduWeb['newestGallery'].onPageChanged;
                var getItemCount = function() { return KoduWeb['newestGallery'].worlds.length; };
                KoduWeb[''].init(onPageChanged, getItemCount);
            }

            KoduWeb['newestGallery'].getWorlds();
        },

        onPageChanged: function()
        {
            KoduWeb['newestGallery'].displayWorlds();
        },

        getWorlds: function () {
            var data = {
                first: 1,
                count: 14,
                sortBy: '0',
                filterBy: '0',
                filterParam: ''
            };
               
            $.ajax({
                'url': '/API/GetWorlds',
                'data': data,
                'type': 'Get',
                'success': KoduWeb['newestGallery'].getWorldsComplete,
                'error': KoduWeb.ajaxError
            });
        },

        getWorldsComplete: function (data) {
            KoduWeb['newestGallery'].worlds = data;        

            KoduWeb['newestGallery'].displayWorlds();

            if (KoduWeb['newestGallery'].hasPagination)
            {
                KoduWeb[''].updatePagination();
            }

            eval('');
        },

        displayWorlds: function() {
            var worlds = KoduWeb['newestGallery'].worlds; 

            var galDiv = KoduWeb['newestGallery'].gallery;
            var galItemTmpl = KoduWeb['newestGallery'].galleryItemTmpl;

            var first = 0;
            var last = worlds.length;

            if (KoduWeb['newestGallery'].hasPagination)
            {
                var currentPage = KoduWeb[''].currentPage;
                var pageSize = KoduWeb[''].pageSize;
                first = (currentPage - 1) * pageSize;
                last = Math.min(worlds.length, first + pageSize);
            }

            var galItems = $(".galleryItem", galDiv);
            galItems.remove();

            if (worlds.length > 0)
            {
                for (var i = first; i < last; i++) {
                    var world = worlds[i];
                    world.GalleryItemNum = i;
                    galDiv.append(galItemTmpl.tmpl(world));
                }

                galItems = $(".galleryItem:nth-child(" + "7" + "n + 1)", galDiv);
                galItems.css("margin-right", "0px");
                galDiv.show();
            }
            else
            {
                galDiv.hide();
            }
        },

        endOfScript: 0
    };

    $(document).ready(function () {
        KoduWeb['newestGallery'].init();
    });
</script>
    



<script id="popularGalleryitemTmpl" type="text/x-jquery-tmpl">


<div class="galleryItem span-3 relative"
    data-itemNum="${GalleryItemNum}"
    >

    <div class="highlight"></div>

    <a class="worldThumbnail gallery block layer-1" href="/world/${World}">
        <img src="/API/Thumbnail?world=${World}" class=""/>
    </a>
    <a class="wrap-1 span-3 layer-1 world-name" href="/world/${World}">${Name}</a>
        <div class="span-3 layer-1 world-creator">
            <div class="left" style="width:15%">by </div>
            <span class="wrap-1 right quiet" style="width:84%" >${Creator}</span>
        </div>
        <div class="layer-1 socl-control rounded-item">
             <img class="socl-image socl-download" src="/content/images/download_white_16.png" />
             <span class="count-value">${Downloads}</span>
        </div>
    <div class="fall-1 span-3"></div>

</div></script>

<script type="text/javascript">
    ///<reference path="Master.js" />

    KoduWeb['popularGallery'] = {
        galleryItemTmpl: $("#popularGalleryitemTmpl"),
        gallery: $("#" + "popularGallery"),
        hasPagination: false,
        worlds: [],

        init: function () {
            if (KoduWeb['popularGallery'].hasPagination)
            {
                var onPageChanged = KoduWeb['popularGallery'].onPageChanged;
                var getItemCount = function() { return KoduWeb['popularGallery'].worlds.length; };
                KoduWeb[''].init(onPageChanged, getItemCount);
            }

            KoduWeb['popularGallery'].getWorlds();
        },

        onPageChanged: function()
        {
            KoduWeb['popularGallery'].displayWorlds();
        },

        getWorlds: function () {
            var data = {
                first: 1,
                count: 14,
                sortBy: '3',
                filterBy: '0',
                filterParam: ''
            };
               
            $.ajax({
                'url': '/API/GetWorlds',
                'data': data,
                'type': 'Get',
                'success': KoduWeb['popularGallery'].getWorldsComplete,
                'error': KoduWeb.ajaxError
            });
        },

        getWorldsComplete: function (data) {
            KoduWeb['popularGallery'].worlds = data;        

            KoduWeb['popularGallery'].displayWorlds();

            if (KoduWeb['popularGallery'].hasPagination)
            {
                KoduWeb[''].updatePagination();
            }

            eval('');
        },

        displayWorlds: function() {
            var worlds = KoduWeb['popularGallery'].worlds; 

            var galDiv = KoduWeb['popularGallery'].gallery;
            var galItemTmpl = KoduWeb['popularGallery'].galleryItemTmpl;

            var first = 0;
            var last = worlds.length;

            if (KoduWeb['popularGallery'].hasPagination)
            {
                var currentPage = KoduWeb[''].currentPage;
                var pageSize = KoduWeb[''].pageSize;
                first = (currentPage - 1) * pageSize;
                last = Math.min(worlds.length, first + pageSize);
            }

            var galItems = $(".galleryItem", galDiv);
            galItems.remove();

            if (worlds.length > 0)
            {
                for (var i = first; i < last; i++) {
                    var world = worlds[i];
                    world.GalleryItemNum = i;
                    galDiv.append(galItemTmpl.tmpl(world));
                }

                galItems = $(".galleryItem:nth-child(" + "7" + "n + 1)", galDiv);
                galItems.css("margin-right", "0px");
                galDiv.show();
            }
            else
            {
                galDiv.hide();
            }
        },

        endOfScript: 0
    };

    $(document).ready(function () {
        KoduWeb['popularGallery'].init();
    });
</script>
    



<script id="highestRatedGalleryitemTmpl" type="text/x-jquery-tmpl">


<div class="galleryItem span-3 relative"
    data-itemNum="${GalleryItemNum}"
    >

    <div class="highlight"></div>

    <a class="worldThumbnail gallery block layer-1" href="/world/${World}">
        <img src="/API/Thumbnail?world=${World}" class=""/>
    </a>
    <a class="wrap-1 span-3 layer-1 world-name" href="/world/${World}">${Name}</a>
        <div class="span-3 layer-1 world-creator">
            <div class="left" style="width:15%">by </div>
            <span class="wrap-1 right quiet" style="width:84%" >${Creator}</span>
        </div>
        <div class="layer-1 socl-control rounded-item">
            <img class="likes-image" src="/content/images/like__white_16.png" />
             {{if (NumLikes > 0) }}
                <span class="count-value likes">${NumLikes}</span>
             {{else}}
                <span class="count-value"> </span>
            {{/if}}
        </div>
    <div class="fall-1 span-3"></div>

</div></script>

<script type="text/javascript">
    ///<reference path="Master.js" />

    KoduWeb['highestRatedGallery'] = {
        galleryItemTmpl: $("#highestRatedGalleryitemTmpl"),
        gallery: $("#" + "highestRatedGallery"),
        hasPagination: false,
        worlds: [],

        init: function () {
            if (KoduWeb['highestRatedGallery'].hasPagination)
            {
                var onPageChanged = KoduWeb['highestRatedGallery'].onPageChanged;
                var getItemCount = function() { return KoduWeb['highestRatedGallery'].worlds.length; };
                KoduWeb[''].init(onPageChanged, getItemCount);
            }

            KoduWeb['highestRatedGallery'].getWorlds();
        },

        onPageChanged: function()
        {
            KoduWeb['highestRatedGallery'].displayWorlds();
        },

        getWorlds: function () {
            var data = {
                first: 1,
                count: 14,
                sortBy: '1',
                filterBy: '0',
                filterParam: ''
            };
               
            $.ajax({
                'url': '/API/GetWorlds',
                'data': data,
                'type': 'Get',
                'success': KoduWeb['highestRatedGallery'].getWorldsComplete,
                'error': KoduWeb.ajaxError
            });
        },

        getWorldsComplete: function (data) {
            KoduWeb['highestRatedGallery'].worlds = data;        

            KoduWeb['highestRatedGallery'].displayWorlds();

            if (KoduWeb['highestRatedGallery'].hasPagination)
            {
                KoduWeb[''].updatePagination();
            }

            eval('');
        },

        displayWorlds: function() {
            var worlds = KoduWeb['highestRatedGallery'].worlds; 

            var galDiv = KoduWeb['highestRatedGallery'].gallery;
            var galItemTmpl = KoduWeb['highestRatedGallery'].galleryItemTmpl;

            var first = 0;
            var last = worlds.length;

            if (KoduWeb['highestRatedGallery'].hasPagination)
            {
                var currentPage = KoduWeb[''].currentPage;
                var pageSize = KoduWeb[''].pageSize;
                first = (currentPage - 1) * pageSize;
                last = Math.min(worlds.length, first + pageSize);
            }

            var galItems = $(".galleryItem", galDiv);
            galItems.remove();

            if (worlds.length > 0)
            {
                for (var i = first; i < last; i++) {
                    var world = worlds[i];
                    world.GalleryItemNum = i;
                    galDiv.append(galItemTmpl.tmpl(world));
                }

                galItems = $(".galleryItem:nth-child(" + "7" + "n + 1)", galDiv);
                galItems.css("margin-right", "0px");
                galDiv.show();
            }
            else
            {
                galDiv.hide();
            }
        },

        endOfScript: 0
    };

    $(document).ready(function () {
        KoduWeb['highestRatedGallery'].init();
    });
</script> 

</body>


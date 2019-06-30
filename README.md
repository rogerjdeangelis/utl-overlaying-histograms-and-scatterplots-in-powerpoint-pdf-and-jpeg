# utl-overlaying-histograms-and-scatterplots-in-powerpoint-pdf-and-jpeg
Overlaying histograms and scatterplots in powerpoint pdf and jpeg
    Overlaying histograms and scatterplots in powerpoint pdf and jpeg                                                       
                                                                                                                            
      Three Solutions  (a;; require R: ppt files require MS Powerpoint )                                                    
                                                                                                                            
            1. Scatter plot with Y and X asis histograms                                                                    
            2. Scatter plot and overlaid histogram                                                                          
            3. Transparency overlay                                                                                         
                                                                                                                            
    Just change the destination if you also want png                                                                        
                                                                                                                            
                                                                                                                            
    github                                                                                                                  
    https://tinyurl.com/y2x33ang                                                                                            
    https://github.com/rogerjdeangelis/utl-overlaying-histograms-and-scatterplots-in-powerpoint-pdf-and-jpeg                
                                                                                                                            
    stackOverflow R                                                                                                         
    https://stackoverflow.com/questions/56822337/overlay-2-images-with-transparency-in-r                                    
                                                                                                                            
    * you need these directories d:/exe/p2p d:/jpg d:/pdf d:/ppt d:/png to hold the output plots;                           
                                                                                                                            
    for output see  github files                                                                                            
                                                                                                                            
    scatter and histogram on top of each other                                                                              
    ------------------------------------------                                                                              
                                                                                                                            
    hissca.jpg                                                                                                              
    hisscat.pdf                                                                                                             
    hisscat.ppt                                                                                                             
                                                                                                                            
                                                                                                                            
    Histograms on margins both x and y                                                                                      
    -----------------------------------                                                                                     
                                                                                                                            
    hismargin.jpg                                                                                                           
    hismargin.pdf                                                                                                           
    hismargin.ppt                                                                                                           
                                                                                                                            
                                                                                                                            
    Transparent  (R logo)                                                                                                   
    ---------------------                                                                                                   
                                                                                                                            
    hismargin.jpg                                                                                                           
    hismargin.pdf                                                                                                           
    hismargin.ppt                                                                                                           
                                                                                                                            
    also in dropbox                                                                                                         
                                                                                                                            
                                                                                                                            
    https://www.dropbox.com/s/so59nboz44y14lb/hissca.jpg?dl=0                                                               
    https://www.dropbox.com/s/7tnx50tqoapdb5g/hisscat.pdf?dl=0                                                              
    https://www.dropbox.com/s/xzgvjctiu99mley/hisscat.ppt?dl=0                                                              
    https://www.dropbox.com/s/q9685mz64b6lj6z/hismargin.jpg?dl=0                                                            
    https://www.dropbox.com/s/gwssaa7lvo7t79b/hismargin.pdf?dl=0                                                            
    https://www.dropbox.com/s/pedig5f78wab7n6/hismargin.ppt?dl=0                                                            
                                                                                                                            
                                                                                                                            
    You need the free BOXOFT pdf_to_ppt product to create the PPTs from the PDFs                                            
                                                                                                                            
    go to                                                                                                                   
    http://www.boxoft.com/pdf-to-ppt/                                                                                       
                                                                                                                            
    I downloaded into d:\exe\p2p                                                                                            
                                                                                                                            
    I tried to subscribe to the newletter but that caused                                                                   
    the install to fail. I installed it at d:exe but                                                                        
    changing the folder name from the default crashed the install.                                                          
    Keep most of the defaults. Copied the install folder contents                                                           
    to d:/exe/p2p                                                                                                           
                                                                                                                            
                                                                                                                            
    Here is the command to create a ppt from a pdf                                                                          
    x "d:\exe\p2p\pdftopptcmd.exe d:\pdf\hissca.pdf d:\ppt\hissca.ppt";                                                     
    The ppt slide will be a bit mapped graphic.                                                                             
                                                                                                                            
    FYI: ghostscript wil allow you to append or insert mutiple pdf pages into one pdf,                                      
                                                                                                                            
    I have posted this, but it is easy.                                                                                     
    The macro on the end will add a theme to the final ppt, however you need allow whitespace                               
    when you create pdf slides.                                                                                             
                                                                                                                            
    One advantage of this method is a pdf slideshow along with a ppt slideshow.                                             
                                                                                                                            
    *_                   _                                                                                                  
    (_)_ __  _ __  _   _| |_                                                                                                
    | | '_ \| '_ \| | | | __|                                                                                               
    | | | | | |_) | |_| | |_                                                                                                
    |_|_| |_| .__/ \__,_|\__|                                                                                               
            |_|                                                                                                             
    ;                                                                                                                       
                                                                                                                            
    * 200 uniform random variables from 0 to 10;                                                                            
                                                                                                                            
    options validvarname=upcase;                                                                                            
    libname sd1 "d:/sd1";                                                                                                   
    data sd1.have;                                                                                                          
      do x=1 to 100;                                                                                                        
        savx=x;                                                                                                             
        y=10*uniform(5731);                                                                                                 
        output;                                                                                                             
        x=10*uniform(5733);                                                                                                 
        output;                                                                                                             
        x=savx;                                                                                                             
      end;                                                                                                                  
      keep x y;                                                                                                             
    run;quit;                                                                                                               
                                                                                                                            
    Up to 40 obs SD1.HAVE total obs=200                                                                                     
                                                                                                                            
    Obs       X          Y                                                                                                  
                                                                                                                            
      1     1.0000    0.20488                                                                                               
      2     5.7843    0.20488                                                                                               
      3     2.0000    3.93098                                                                                               
      4     6.1364    3.93098                                                                                               
      5     3.0000    7.04374                                                                                               
      6     9.2849    7.04374                                                                                               
                                                                                                                            
    * you need this executable to covert pdf to ppt;                                                                        
    x "d:\exe\p2p\pdftopptcmd.exe d:\pdf\hissca.pdf d:\ppt\hissca.ppt";                                                     
                                                                                                                            
    *            _               _                                                                                          
      ___  _   _| |_ _ __  _   _| |_                                                                                        
     / _ \| | | | __| '_ \| | | | __|                                                                                       
    | (_) | |_| | |_| |_) | |_| | |_                                                                                        
     \___/ \__,_|\__| .__/ \__,_|\__|                                                                                       
                    |_|                                                                                                     
    ;                                                                                                                       
    ...                                                                                                                     
                                                                                                                            
    1. Overlay a scatter plot and histogram)                                                                                
    ===========================================                                                                             
                                                                                                                            
    EXAMPLE 1                                                                                                               
    ---------                                                                                                               
                                                                                                                            
       Y |                                                                                                                  
         |                                                                                                                  
    10.0 +  ** *               *               *           |                                                                
         | *  **     **                        *           |                                                                
         |  ****         * *   *    **  *  *               |*********                                                       
         | *** *         *   *  *            *             |                                                                
         | ****   *         *                    *         |*********                                                       
     7.5 + * ** **     *         * *      *       *        |                                                                
         |  ****           *  *      *          *          |*************                                                   
         |   **                    *   *         *         |                                                                
         | *  *     *                      *               |********                                                        
         |  ** *       *  *     *                          |                                                                
     5.0 +  ***                     *   *        *         |*******************                                             
         |  ***  *                 *     *                 |                                                                
         | *****       *         *    *  *   *  *          |********                                                        
         |  ****  ****                      * *   *        |                                                                
         |   * *        *                                  |******                                                          
     2.5 +  * *  *   *           *        **               |                                                                
         |  * *                   *         *              |**************                                                  
         |   **         *             **      *    *       |                                                                
         | ** *          ** **    *                        |**************                                                  
         | * ****  *       * **        *     *             |                                                                
     0.0 + * **       *        *     *             *       |*********                                                       
         |                                                 |                                                                
         --+---------+---------+---------+---------+-      -----+----+----+----                                             
           0       2.5        5.0       7.5      10.0          10   20    30                                                
                                                                                                                            
      10 +  ****  ****  ****  ****  ****  ****  ****                                                                        
         |  ****  ****  ****  ****  ****  ****  ****                                                                        
         |  ****  ****  ****  ****  ****  ****  ****                                                                        
         |  ****  ****  ****  ****  ****  ****  ****                                                                        
         |  ****  ****  ****  ****  ****  ****  ****                                                                        
      20 +  ****  ****  ****  ****  ****  ****  ****                                                                        
         |  ****  ****  ****  ****  ****        ****                                                                        
         |  ****  ****  ****  ****  ****        ****                                                                        
         |  ****  ****        ****              ****                                                                        
         |        ****        ****              ****                                                                        
      30 +        ****        ****              ****                                                                        
         |        ****        ****              ****                                                                        
         |        ****        ****              ****                                                                        
         |                    ****              ****                                                                        
         |                    ****                                                                                          
                                                                                                                            
                                                                                                                            
    EXAMPLE 2                                                                                                               
    ---------                                                                                                               
                                                                                                                            
    10 +                                                                                                                    
       |          *                    *    GGG                                                                             
       |          *     * *   *             GHG                                                                             
       |              *         FFF    *  * HHH                                                                             
       |*                       GGG      *  GGG                                                                             
       |   *    *               GGG         GGG                                                                             
       |                   *    GGG *       GGG                                                                             
     5 +    *       DDD         GGG         HGG                                                                             
       |*         * GGG         GGG    *    GGG                                                                             
       |            GGG     *   GGG         GGG                                                                             
       |    *  *    HHH         HHH         HHH                                                                             
       |CCC         GGG         GGG         GGG                                                                             
       |GGG         GGG         HGG   *     GGG                                                                             
       |GGG       * GGG         GGG         GGG                                                                             
     0 +DDD         DDD         DDD         DDD                                                                             
       |                                                                                                                    
       -+---------+---------+---------+---------+-                                                                          
       0         2.5       5.0       7.5      10.0                                                                          
                                                                                                                            
                            X                                                                                               
                                                                                                                            
    EXAMPLE 3                                                                                                               
    ---------                                                                                                               
                                                                                                                            
    G green dot                                                                                                             
    R red dot                                                                                                               
    B blue dot                                                                                                              
    Y yellow dot                                                                                                            
                                                                                                                            
    +---------------------+                                                                                                 
    |        ____   Y     |                                                                                                 
    |    R  |R _ \      B |                                                                                                 
    |    Y  | |_)B|  G B  |                                                                                                 
    | R     |B _ <        |                                                                                                 
    |    C  |_| \_\ Y     |                                                                                                 
    |                     |                                                                                                 
    +---------------------+                                                                                                 
                                                                                                                            
    *          _       _   _                                                                                                
     ___  ___ | |_   _| |_(_) ___  _ __  ___                                                                                
    / __|/ _ \| | | | | __| |/ _ \| '_ \/ __|                                                                               
    \__ \ (_) | | |_| | |_| | (_) | | | \__ \                                                                               
    |___/\___/|_|\__,_|\__|_|\___/|_| |_|___/                                                                               
                                                                                                                            
     _                                _             _     _     _                                                           
    / |     _ __ ___   __ _ _ __ __ _(_)_ __       | |__ (_)___| |_                                                         
    | |    | '_ ` _ \ / _` | '__/ _` | | '_ \ _____| '_ \| / __| __|                                                        
    | |_   | | | | | | (_| | | | (_| | | | | |_____| | | | \__ \ |_                                                         
    |_(_)  |_| |_| |_|\__,_|_|  \__, |_|_| |_|     |_| |_|_|___/\__|                                                        
                                |___/                                                                                       
    ;                                                                                                                       
                                                                                                                            
    * you need these directories d:/jpg d:/pdf d:/ppt;                                                                      
                                                                                                                            
    * delete all outputs;                                                                                                   
    %utlfkil(d:/jpg/hismargin.jpg);                                                                                         
    %utlfkil(d:/pdf/hismargin.pdf);                                                                                         
    %utlfkil(d:/ppt/hismargin.ppt);                                                                                         
    %utlfkil(d:/jpg/hisscat.jpg);                                                                                           
    %utlfkil(d:/pdf/hisscat.pdf);                                                                                           
    %utlfkil(d:/ppt/hisscat.ppt);                                                                                           
                                                                                                                            
    %utl_submit_r64('                                                                                                       
    library(psych);                                                                                                         
    jpeg("d:/jpg/hismargin.jpg");                                                                                           
    data(sat.act);                                                                                                          
    with(sat.act,scatter.hist(SATV,SATQ));                                                                                  
    dev.off() ;                                                                                                             
    pdf("d:/pdf/hismargin.pdf",7,5);                                                                                        
    with(sat.act,scatter.hist(SATV,SATQ));                                                                                  
    dev.off() ;                                                                                                             
    ');                                                                                                                     
                                                                                                                            
    x "d:\exe\p2p\pdftopptcmd.exe d:\pdf\hismargin.pdf d:\ppt\hismargin.ppt";                                               
                                                                                                                            
    *____       _     _     _                      _                                                                        
    |___ \     | |__ (_)___| |_      ___  ___ __ _| |_                                                                      
      __) |    | '_ \| / __| __|____/ __|/ __/ _` | __|                                                                     
     / __/ _   | | | | \__ \ ||_____\__ \ (_| (_| | |_                                                                      
    |_____(_)  |_| |_|_|___/\__|    |___/\___\__,_|\__|                                                                     
                                                                                                                            
    ;                                                                                                                       
                                                                                                                            
    * could add or have appropriate histogram access - too lazy;                                                            
    %utl_submit_wps64('                                                                                                     
    libname sd1 "d:/sd1";                                                                                                   
    options set=R_HOME "C:/Program Files/R/R-3.5.1";                                                                        
    libname wrk "%sysfunc(pathname(work))";                                                                                 
    libname hlp "C:\Program Files\SASHome\SASFoundation\9.4\core\sashelp";                                                  
    proc r;                                                                                                                 
    submit;                                                                                                                 
    source("C:/Program Files/R/R-3.3.2/etc/Rprofile.site", echo=T);                                                         
    library(haven);                                                                                                         
    a<-read_sas("d:/sd1/have.sas7bdat");                                                                                    
    jpeg("d:/jpg/hissca.jpg");                                                                                              
    hist(a$Y, xlim=c(0,10),yaxt="n",ylab="",xlab="");                                                                       
    par(new=TRUE);                                                                                                          
    plot(a,xlim=c(0,10), add=T,pch = 3);                                                                                    
    dev.off();                                                                                                              
    pdf("d:/pdf/hisscat.pdf");                                                                                              
    hist(a$Y, xlim=c(0,10),yaxt="n",ylab="",xlab="");                                                                       
    par(new=TRUE);                                                                                                          
    plot(a,xlim=c(0,10), add=T,pch = 3);                                                                                    
    dev.off();                                                                                                              
    endsubmit;                                                                                                              
    run;quit;                                                                                                               
    ');                                                                                                                     
                                                                                                                            
    x "d:\exe\p2p\pdftopptcmd.exe d:\pdf\hisscat.pdf d:\ppt\hisscat.ppt";                                                   
                                                                                                                            
    *_____     _____                                               _                                                        
    |___ /    |_   _| __ __ _ _ __  ___ _ __   __ _ _ __ ___ _ __ | |_                                                      
      |_ \      | || '__/ _` | '_ \/ __| '_ \ / _` | '__/ _ \ '_ \| __|                                                     
     ___) |     | || | | (_| | | | \__ \ |_) | (_| | | |  __/ | | | |_                                                      
    |____(_)    |_||_|  \__,_|_| |_|___/ .__/ \__,_|_|  \___|_| |_|\__|                                                     
                                       |_|                                                                                  
    ;                                                                                                                       
                                                                                                                            
    %utl_submit_r64('                                                                                                       
    library(jpeg);                                                                                                          
    library(abind);                                                                                                         
    img.logo = readJPEG(system.file("img", "Rlogo.jpg", package="jpeg"));                                                   
    img.logo = abind::abind(img.logo, img.logo[,,1], along=3);                                                              
    img.random = img.logo;                                                                                                  
    img.random[] = runif(prod(dim(img.random)));                                                                            
    img.logo[,,4] = 0.5;                                                                                                    
    img.random[,,4] = 1;                                                                                                    
    pdf("d:/pdf/transparent.pdf", width = 2, height = 2);                                                                   
      par(mai=c(0,0,0,0));                                                                                                  
      plot(1:2, type="n", xaxt="n", yaxt="n", bty="n", xlab="",ylab="");                                                    
      rasterImage(img.random, 1, 1, 2, 2);                                                                                  
      rasterImage(img.logo, 1, 1, 2, 2);                                                                                    
    dev.off();                                                                                                              
    jpeg("d:/jpg/transparent.jpg");                                                                                         
      par(mai=c(0,0,0,0));                                                                                                  
      plot(1:2, type="n", xaxt="n", yaxt="n", bty="n", xlab="",ylab="");                                                    
      rasterImage(img.random, 1, 1, 2, 2);                                                                                  
      rasterImage(img.logo, 1, 1, 2, 2);                                                                                    
    dev.off();                                                                                                              
    ');                                                                                                                     
                                                                                                                            
                                                                                                                            
    x "d:\exe\p2p\pdftopptcmd.exe d:\pdf\transparent.pdf d:\ppt\transparent.ppt";                                           
                                                                                                                            
                                                                                                                            

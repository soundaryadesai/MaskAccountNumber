# MaskAccountNumber

        String str = "25462|626562|2385853285397|Y|NA"; 
        String[] arrOfStr = str.split("\\|"); 
         String accNo = arrOfStr[2];
         System.out.println(accNo);
         
         String maskNo="";
// maskNo = accNo.substring(0, accNo.length() - 4).replaceAll("[0-9]", "X").concat(accNo.substring(accNo.length() -4));
// System.out.println(maskNo);  

         for(int i=0;i<accNo.length();i++) 
         {
        	 if(i<accNo.length() - 4)
        	 {
        		 maskNo += "X";
        	 }
        	 else
        	 {
        		 maskNo += accNo.charAt(i);
        	 }
        	 
         }
         System.out.println(maskNo);
       
P

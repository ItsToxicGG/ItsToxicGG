  ## HI IM ITZTOXIC
  
![ItzToxic's github stats](https://github-readme-stats.vercel.app/api/?username=ItsToxicGG&show_icons=true&hide_border=true&theme=algolia&count_private=true)
[![Top Langs](https://github-readme-stats.vercel.app/api/top-langs/?username=ItsToxicGG&show_icons=true&hide_border=true&theme=algolia&count_private=true)](https://github.com/ItsToxicGG)

```php

<?php

namespace profile;

use profile\ItsToxicGG;
use github\utils\Color;


class Credits extends GitCredits{
    
    public $credits;
    
    public $cname = "{RED} Error code 41: This is caused because it could not find the correct name!"
    
    public function credits($credits){
        $credits = "Toxics Stats Credit to $cname";
    }
    
}
   
```

```php

<?php

namespace profile;

use profile\credits
use github\profile\ProfileBase;
use github\profile\Restore;
use github\utils\Color;
use github\profile\Account;

class ItsToxicGG extends ProfileBase{
   
   public $name;
   public $gitcredit;
   public $gmail;
   public $discord;
   public $favsongs;
   public $languages;
   public $contry;
   public $register = "register, $name, $gmail, $discord, $favsong, $languages";
   public $staff = "james, david, kay, lee, jordon";
   public $error21 = "{RED} Error code: 21, This is caused of bad connection to the server!";
   public $error136 = "{RED} Error code: 136, This is caused because your profile is not yet done!"
   
   public function profilesend(){
       echo "im $name";
       echo "contact me: $gmail";
       echo "chat with me: $discord";
   }
   
   public function registerProfie(string $name, string $password, string $email);
       session_start();
       $register = new Account($this);
       $register->setPassword($password);
       $register->addPassword($register->inputPasswordFromForm());
       $register->getAndSetName($register->inputNameFromForm($name));
       $register->removeEmailByName("@waitingfornewprofile.com");
       $register->addNewEmailByInputForm(Restore::getEmail()->getInput($gmail));
    }
    
    public function onProfileDelete(){
        session_end();
        session_unset();
        $profile = $this->registerProfile($name, $password, $gmail);
        $register = new Account();
        $register->unsetAccount();
        $register->getHack()->hackMysqlData()->getDataOfDeletedProfile()->getDataNamePasswordEmail();
        $register->setAllInputs(" ");
        $register->setInputEmail("@waitingfornewprofile")
    }
    
    public function restoreDeleteProfile(Restore $restore): void{
        session_start();
        if($restore->mysqlolddata === null){
            $restore->getEmail()->getMysqlData()->deleatedInfo()->getEmailByOldDataKept($restore->email);
        } else {
            $restore->getEmail()->getHack()->hackInMysql()->getDeletedAccountDetials()->getOldInputofGmail($restore->email);
        }
        $restore->getName()->getHack()->onName()->retoreByName($restore->addRestoreInputOnName($restore));
        $restore->getName()->restorePasswordByName()->getLSHack()->restorePasswordOfName($restore->addRestoreInputOfPasswordByName($restore));
    }


```

```php
<?php

namespace profile;

use profile\ItsToxicGG;
use github\profile\ProfileUtils;

class ProfileUtils extends ProfileUtils{
// soon!
}

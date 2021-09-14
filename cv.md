# CV of Yuliya Mititel #

## Contact information ##

* *Phone:* **89036897649** 
* *Email:* **[yulia.mititel@yandex.ru](mailto:yulia.mititel@yandex.ru)**
* *Telegram:* **@yuliya_mititel**


## Skills ##
1. HTML
1. CSS
1. GIT
1. SQL
1. Java Script basics

### Code ###
    function toReadable (number) {
    const strNumber=String(number);
    const arrNumber=strNumber.split('');
    console.log(arrNumber);
      const lenNumber=strNumber.length;
      const arrWords= ['zero', 'one', 'two', 'three', 'four', 'five', 'six', 'seven', 'eight', 'nine', 'ten', 'eleven', 'twelve', 'thirteen', 'fourteen', 'fifteen', 'sixteen', 'seventeen', 'eighteen', 'nineteen']; 
    const decades=['twenty', 'thirty', 'forty', 'fifty', 'sixty', 'seventy', 'eighty', 'ninety'];
    const hundred=['one', 'two', 'three', 'four', 'five', 'six', 'seven', 'eight', 'nine'];
    let wordNumber=[];
      switch (lenNumber) {
            case 1:
                 wordNumber[0]=arrWords[number];
                break;
            case 2:
                if (number <= 19) {
                    wordNumber[0]=arrWords[number];
                } else {
                    wordNumber[0]=decades[arrNumber[0]-2];
                    if (number%10!==0) {
                    wordNumber[1]=arrWords[arrNumber[1]];
                    }
                }
                break;
            case 3:
                wordNumber[0]=hundred[arrNumber[0]-1]+ ' hundred';
              let decWordNumber=Number(strNumber.substr(-2));
              if (number%100!==0) {
                  if (decWordNumber<=19) {
                    wordNumber[1]=arrWords[decWordNumber];
                  } else if (decWordNumber % 10===0) {
                    wordNumber[1]=decades[arrNumber[1]-2] ;
                    } else {
    wordNumber[1]=decades[arrNumber[1]-2];				
    wordNumber[2]=arrWords[arrNumber[2]];
                  }
              }
                break;
        }
    return wordNumber.join(' ');}
    


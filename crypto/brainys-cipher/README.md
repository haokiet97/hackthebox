# Crypto Challenge: Brainy's Cipher (30 Points)

**Brainy likes playing around with esoteric programming. He also likes math and has therefore encrypted his very secure password with a popular encryption algorithm. Claiming that his password cannot be retrieved now, he has sent the ciphertext to some of his friends. Can you prove to Brainy that his password can actually be recovered?**

This challenge gave us a file named brainy.txt.

```
$ cat brainy.txt 
++++++++++[>+>+++>+++++++>++++++++++<<<<-]>>>>+++++++++++++++++++++++.-----------.<------------.---.++.---------.+.++.-.++.+.-----.++..++++.--.++++.+..-------.+.+++.---.+.+++++.-------.+.---.+++++++.+.-------..+++.-.+++++.-------.++.+++++.-----.+++++..-----.--.++++++++.-------.--.++++.+++.---.++..+++.------.+++.--.-..++++++.-.----..+++++.------.++++++.---.---.--.+++.++++.-------.+++++..-.++..-------.++++++.---.++..+++.----.++++.-------.++++++++..----.+++.+.------.--.-.++.-.+++++.--..--.++++.-.++++.---.------.+++++.++.+.---.+++.---.----.++++.--.+++.-----.+++++.+.---.--.+++++++.---.---...---.+.++++++++.----.++++.-----.++.--.-.--.++.-.-.+++++.--..+++++.-------.-.++++.++.-----.++++++.--------.+++.+++.-.+++.----.----.++++++.----.++++++.-------.-----.>+.<++++++++++++++.---------.+.++++++.--------.++.+++++++.--------.+++++++.----.+.----.+++...----.++++..++.----..+++.+++.-----.++++.--.++..-------.+++.++++.--.---.--.++++++..-----..+++++++.-------.+++++++.--------..++++++.++.--..++.----.+++.++.------.++++.+.-..+.+.-------.++++++.-.---.---.-.++++++++..-----.---.++.+.++..-.--.+++.++++.--..------.++++++++.-------.+++++++..---.+.++..---.----.+.++++++..-.-.-----.--.++++.--.+++++++.----.++++.-----.-.+.++.+..+..--.-.---.+++++.--.--.++++++.--------.++.---.+++++++..----.---.+++++++++.-...-------.++++++++.-------.++.-.+++++.----.-.+++++.---.----.+++++.++.-----.---.+++++++.++.---------...++.+++++++.------.+++++.-------.++++.-----.+++++.----.-----.>-------------.++++++++++++.<++++++++++++++.-----..-.----.++++++.-..-----.++.++++++.--.----..--.++.-.++++++++.------.+..--.+++++++.------.---.++++++.----.++++++.-.++.------.++++...--.---.+++++++.--------.++++++++.----..+.----.+..---.++++++++.+.---.-.---.--.++++++++.-----.+++++.----.+.+++.------.--..+++++++++.-.---.++.----.++++.-.------.+++++.--.++.+++.-----.++.++.--..----.-.+++++++.+.----.---.+++++.+++.---.-----.+++++.------.++++++.-.----..++.+++.--.---.++.++++++.--------..+++++.+++.---.-----.++.++++++.---.+++.-.-------.++.+++.-.---.+++.---.+.++.-----.+++++++.---.--.-..++++.++.-------.++++.+.--.++++..+.+.-.---.-.--.+.+++++.--.+++.------..--.++++++++.-.------.++++.+++.-----.+.----.-----.>------------.+++++++++++++.<++++++++++++++.-.---------.++++++..++.+.--.----.-.--.+++.---.++++++++..-----.+.--.--.++++++.+++.----.---.+.++.++++.------.++++++..--.----.++++..---.+++.----.--..++++++++.-.-----..---.+++++++++.---------.++++++.----.+++++.-.--.---.++++++.+.+.---------.++++++.----.++++.+++.-----.+++.--.+++.----.+++.------.++++++.----.++++++.---..------.+++++++.----.++.+.+.++.-..-------.++++++.-------.++++.---.++++.+++.-----.++++++..----.-.+++++..---.---.-..+.--.+++.---.++++.++.---.-.+++++.-..-------.++..+++.++++.----.---.++.+++++.--------.++++.+.------..+++++.---.++++++.-.------.+++.++.--.---.++.+++.-----.+++++.---.+.--.-.+++++++.+.-------.--.+++++.-----..+++++.++.---.+++++.-.--.-.----.-----.>--------------.<++++++++++++++.----.----.--.+++++++.+.--------.++++++++.--..+..---.---.+++++..++.--.++.--.+.------.+++++++.-----.+++++.---.++.++.----.++.----.++.-----.+++..+++++.-----.--.+++...++.----.++++++.--------.+++++++++.--------.+.++++.+.----..++++++.-------.++..++++.--------.++++++.-.-----.++.++++.++.---.-----.++.-.+.++++.++.---.--.-.++++.-..----..+++++++.-----.++++++.---.----.--.+++++.+.--.+++++.----.++++.---.--.+.++.++.--.+.------.+.-.+++.--.---.++.--.++++++++.------.--.+++++.-.-.++++++.------.++++++.------..+++.++.------..++++.-.++..-----.++++++.--------.++.+++++.--.-----.++++++++..-.-----.+++++++.------.+++.------.++.++.-.-.+++.----.+.+++++++.---.+.++..-----.++++.--------.+++++..-.+++++..---.-.-----.++.--.+++++++++.--------.+++++.+++.----.--.+++.--..++.---.++.++++.---.-.++++.--------.+++++..------.+++++++.++.-------.+++.--..++.+.---.++++++.---------.++.+++++.--.++.++.--------.+++++++.-.---.-.++.----.+++++++.--------.++++++.------.+++++++.---.+++.--.++++.---.---..-..++.++.-.-.---.++++++..--.+++.+.----.++++.---------..++.+.+++++.---.-.+.----.+++++++.--.---.--.+..-.-.++++++.--.++++.-.+.-----.+.+++.+.----.++.++..--------.++.+++++++.--------.+++++.+..-----.--.+.++++++.--.----.+.++++++.--------.++++++++.------.--.++++++...+.-------.+++++++++.-----.+.+.----.+++.-----.++++++.+.+.--------.+++.+++++.-------.+.+++++++.--.-------.++++++++.-.------.>++++++++++++++++++++++++++.
```

The content of the file is very familiar for me. Oh, that is Brainfuck Language!

We can use this website https://copy.sh/brainfuck/ to translate the message. 

```
{
  p:7901324502264899236349230781143813838831920474669364339844939631481665770635584819958931021644265960578585153616742963330195946431321644921572803658406281,
  q:12802918451444044622583757703752066118180068668479378778928741088302355425977192996799623998720429594346778865275391307730988819243843851683079000293815051,
  dp:5540655028622021934429306287937775291955623308965208384582009857376053583575510784169616065113641391169613969813652523507421157045377898542386933198269451,
  dq:9066897320308834206952359399737747311983309062764178906269475847173966073567988170415839954996322314157438770225952491560052871464136163421892050057498651,
  c:62078086677416686867183857957350338314446280912673392448065026850212685326551183962056495964579782325302082054393933682265772802750887293602432512967994805549965020916953644635965916607925335639027579187435180607475963322465417758959002385451863122106487834784688029167720175128082066670945625067803812970871
}
```

The translated message is very familiar to me and I know this is some kind of RSA challenge. So using the python script uploaded here, I was able to decode it and get the flag.

```
$ python rsa-solver.py 
Qinv: 220704337201952911765675653562663630182944011601434480318719267734294597214029345583566925914822207084641554600189204004345080805963023444063892299263948
m1: 49437413074993986257824490238275931180994249527518860068137626874351971280859988288289074
m2: 49437413074993986257824490238275931180994249527518860068137626874351971280859988288289074
h: 0
m: 49437413074993986257824490238275931180994249527518860068137626874351971280859988288289074
solved: ch1n3z_r3m4ind3r_the0rem_r0ck$$$_9792
```


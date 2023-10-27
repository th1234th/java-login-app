## Java Login App ##
Project based on [dptrealtime](https://bitbucket.org/dptrealtime/java-login-app/src/master/)

## We are using docker, maven, mysql, nginx and tomact
![Schema app](https://lh3.googleusercontent.com/pw/ADCreHc1K0_NQEkSHY79tK4oNpG6FF40jgWh2NUEHQXIun2WAeqP_os9ijZSCJSNSVNOqHCifuus6T-jEXH7ZWC6LJXQ1-Wj130jWcK1nLew17o7d7TF00_E75T5yY3ff5SBrmVJUCMlK5o8Qwtc17EOVZ5yRqIBoTnYUnz1fLill13A9qt2IPII19PtihwlOJE8cTM0W6-mRT7CDNMtzlYsnwV_n6UEW6Q2gGKdO36pZlIFeEQmcQhgVhituFMbfRHvz9eTvMmgS9NQcMOkoDItr1Tq1_JyMLmreqQP5kf5ltykwqgr6IxUEmv63WIlXVG5X9ys4cs9J1_KhHSp_FP12n6g6XVKsSvj7Up-yfNXnydRg88Wry56DEBO2PrxPV5n-gsyfwAhpVQDA5jGLc7hUFe6_IrdW0sbN8iz6LYpmhXKMAkjfESkF2P329chYvsDMKY7NANS8qcJHYfbYiLxVFoWDOrW4thscIdUv8ZDNj7-RqE81T77ytODGCl9ImKzw2ybNtxGthSgjvcDlhBblz0mZply5qRpdJvPDU2VF_AocbQQfnTE0gk_ZG7LGSg9pgpYHmdQh2mens8USG7jNPKQJ84dnNVoHia9B9OE4uJnW5C8pV1R7llVEkxepL-YlsJySuq-VS3IYPxgh3kvE2bG4DvB1ZQhqckud40hEoIcSPpfTQGuHsg-LFSd0dmGfqxBKdDpgwfIR1sTK3eMjutQxMMs3MS-fRF31f0Zq5p7Z0wmyDuzjhomIliE0Eb8N7ame9NBfPOn5QtBmZJ5shIOZYjxLlN7Xabqo__A24-mBnncLui2peddOh7yiSPe8lYVwopgMb1bDvNFvSdj-skl1Cta-7lP1Jv4o_F6fnDiWdJR5ytIZcWx44-twR8rpXPowE8GmJ0yDQMP-4xTn-NooBHDleuOzjSB3nxCRg7HjHzbMC-GwfqHFDKsqO6x2POvvLwt_ipPi1QxXLtqW2PKhf0UCV9E3hIfZrvCSNyy5NzZlHukuoqy1gODFDPSCLuYzjGxaQv9l-dOqrF0wYEmapPUCQAaLDP1kOAA815rKCxDi3-4W-Ki_SC-NZMk7qub3vq7=w1920-h937-s-no-gm?authuser=1)


## How to create Table ##
## Below Query to create require TABLE schema to store Employee records ##
## You can create after the running container bd but the most efficient way is to create a init.sql script file 
## and copy it in docker-entrypoint-initdb.d/ 

```
CREATE TABLE Employee (
  id int unsigned auto_increment not null,
  first_name varchar(250),
  last_name varchar(250),
  email varchar(250),
  username varchar(250),
  password varchar(250),
  regdate timestamp,
  primary key (id)
);
``` 


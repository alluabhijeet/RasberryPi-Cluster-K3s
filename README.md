# RasberryPi K3s Cluster

![thumbnail_IMG_0686](https://github.com/alluabhijeet/RasberryPi-Cluster-K3s/assets/120827058/71dae4e6-5cfe-4bee-a7b1-02f4fafdc2f2)


## Hardware
- Two [RasberryPi 4 8GB RAM Boards](https://www.adafruit.com/product/4564?gad_source=1&gclid=CjwKCAjw9IayBhBJEiwAVuc3fjbqRDsdYKR40A5_c4Br_HfWsGAFc4f4b_7HfMdmpjcUxgTHrcQPDRoCBD0QAvD_BwE). One for Control Node and one for Worker Node
- [Two 256 GB SD Cards](https://www.amazon.com/Silicon-Power-Superior-microSDXC-MicroSD/dp/B07S5T7YR5/ref=sr_1_9?crid=LX5GQUEPQF1V&dib=eyJ2IjoiMSJ9.q_hkKbTyrfHvoWrPjalRApbJzmeyFlSt-bHQHB5p7Vea0IxWuG3G-MZqEcFTAfpU9wXOwSG1ftDGpTw2osTqG1r5kzFwXjGLHgQN7gkIXEsz_q8F8SaRb2mdkEMQtFPCPOcSJ-I-T7g-TM_qwx-AicVuvO6v-0TAJbWGUznBS9Wyo84itP4huoA1Bw02nBeJ3dri5VhDEZQfpNXjN_wgLu_9UYxU9wWKCqb-PgIdiKFcHv1acWacjHXGToWsNO1mik8_pcDBcTtjFD8MvgQYBFhiPoXqd6ROe8d_rdXIadI.tNXpC4lvayCAjBKM7yekB6qd71EEnua7uCrYE_GE-IU&dib_tag=se&keywords=Micro+SD+Memory+Cards+256&qid=1715611243&s=pc&sprefix=micro+sd+memory+cards+256%2Ccomputers%2C147&sr=1-9)
- [Anker Power Station to power the boards](https://www.amazon.com/Anker-Charger-PowerPort-iPhone-Galaxy/dp/B00P936188/ref=sr_1_3_pp?dib=eyJ2IjoiMSJ9.KGMmSlNQ2c4nROepIfQ0r3TYxZPMLOJnQraY2tbdElYnYAstTn8U9J3n0B8dmaA7jcIAbZMJBbc20qDkt_fS7yeC6NmdVFsk62ilrgpi7NgA8UuBOwu6CyHawcj8PetwsxudaralQexrNlqyAbJE9oYSBWxMaQ-at-nUCWXVpS-ZVrbA0IjuJWMGAEv6LLXqniUaa9Ww4JejgeOvw4Upstxy1Ssku3kh39bH6ES5Xxg.npA1K96HHnNHqSWqUkpF7pAj_PpyfE6RcxuDFkpZriQ&dib_tag=se&keywords=anker+power+station&qid=1715611321&sr=8-3)
- [Ethernet Cables](https://www.amazon.com/Ethernet-Higher-Bandwidth-Internet-Network/dp/B0CHYH5TYC/ref=sr_1_11?crid=32EBDWTWCBEAX&dib=eyJ2IjoiMSJ9.fDWGdDb_H38FJeS_g9LF_p5TT8FtVJSuQgr60i3EjfW1HSJXKahreqxGXetlBnAf5W_FFhqg9DNUTQFGJeYM9h9zx7a9JjjB9e31tJ7nKi0K9NKi_SrtA4r_Y0jRqBplQQjAl_CiSFV46BWfw2ML6mHmeNHD7WWtD2PMmChtgby0zxekmWJBI_mx1JSBitoToLMA7SKrL7tyUh696ZuWFHokrP_YYesb7OqgKWIZFdc.DtRlxfTSFdUUJ0Cq3UwrdwUz5C8qVBQjLMEEdHkNGDw&dib_tag=se&keywords=ethernet%2Bcable%2Bshort&qid=1715611381&sprefix=ether%2Bcable%2Bshort%2Caps%2C127&sr=8-11&th=1)
- [Ethernet Switch](https://www.amazon.com/TP-Link-5-Port-Gigabit-Network-Switch/dp/B0863M7C1L/ref=sxin_13_recs_zoco_stores_brand_identity_bs?content-id=amzn1.sym.7d2e00dd-9358-4f89-aca0-04685eb73811%3Aamzn1.sym.7d2e00dd-9358-4f89-aca0-04685eb73811&crid=3HV7V8D93F5YZ&cv_ct_cx=ethernet+switch+tp+link&dib=eyJ2IjoiMSJ9.YuvgVwjxryUNqZpw3Tz1GDmtOjn0hvMIuE2UTOfgHUMjlNFngtLCPlT-NrsnCTtRQjw03zNXfDITy-YXK9YX4opcHuHiBQ46RWG0Psiskff7UQZhjH74KptcCet5vGP8.DjmBoJCwCVv4ThNGqgZXnNgCmxREbZFB5fq9So1GZzI&dib_tag=se&keywords=ethernet+switch+tp+link&pd_rd_i=B0863M7C1L&pd_rd_r=a8d84e0f-267e-4747-a9c6-c46a1e693826&pd_rd_w=r464B&pd_rd_wg=3rZDt&pf_rd_p=7d2e00dd-9358-4f89-aca0-04685eb73811&pf_rd_r=097NS0XK29T7MH52D9H2&qid=1715611500&sbo=RZvfv%2F%2FHxDF%2BO5021pAnSA%3D%3D&sprefix=ethernet+switch+tp+link%2Caps%2C127&sr=1-5-5f457e4f-4cf5-45bd-948b-58563dcb013a)
- [Cluster Case](https://www.amazon.com/GeeekPi-Raspberry-Cluster-Cooling-Heatsink/dp/B07MW3GM1T/ref=sr_1_57?crid=1QFPKHSBHJL86&dib=eyJ2IjoiMSJ9.lZ-H4wnPfjUWX4rszBeKlVqVk6XPxpgJAcgENG-_Psq3B_gBlfqZCosZXZO7x6kD38FP7-MvFLOswAtVJGRQTTQKVlvQwDYh9KGmAxWhkm03S_TcFYXD5N_uuH6D9A9LV5yjZkgg8sOmUKMjTpale8E5TKKKALvfvnijaqRCWsc.MzaeB80ww7vo52wJSIfSjBsJIvHBFqYkwq3fnd0oPDA&dib_tag=se&keywords=raspberry+pi+4+cluster+case&qid=1715611627&sprefix=rasberry+pi+4+cl%2Caps%2C133&sr=8-57&xpid=v5SDtPVt83LJ_)

## Software
- Two boards are running Ubuntu Server 24.04. The OS was flashed to the SD card using the RasberryPi Imager.
- K3s was deployed to the cluster using official Ansible Role from Rancher Labs, with slight modifications.
- K3s has a default flannel CNI, but I opted out of it and installed Cilium.

## Useful Links 
- [Ansible Role](https://github.com/k3s-io/k3s-ansible)

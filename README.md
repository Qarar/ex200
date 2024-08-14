This video is discussing Question 13 of the RHCSA Redhat Exam200, which is related to PodMan.If the video quality is slow, try changing the resolution.
Access All question from this course
https://www.udemy.com/course/redhat-ex200-rhcsa-exam-2024-april-06/?couponCode=KEEPLEARNING

Watch this video to understand the question

https://www.youtube.com/watch?v=pg8P6t9P_3M

 useradd alth
 passwd alth 
 ssh-keygen 
 ssh-copy-id -i /root/.ssh/id_rsa-pub alth@localhost
 /root/.ssh/id_rsa.pub 
 ssh-copy-id -i /root/.ssh/id_rsa.pub alth@localhost
  ssh alth@localhost
 Answer start from here
From root user
Yum install podman* -y
systemctl start podman.service
systemctl start podman.socket
systemctl enable podman.service
systemctl enable podman.socket
mkdir /opt/file
mkdir  /opt/outprocess
chown alth:alth /opt/files
chown alth:alth /opt/processed/
ssh alth@localhost
podman run -dit --name asciipdf -v /opt/files:/opt/incoming:Z -v /opt/processed:/opt/outgoing:Z monitor

mkdir -p .config/systemd/user
cd ~/.config/systemd/user
podman generate systemd --name asciipdf --new  - -iles
systemctl --user daemon-reload

systemctl --user start container-asciipdf.service
systemctl --user enable container-asciipdf.service

systemctl --user enable container-asciipdf.service
loginctl enable-linger
loginctl show-user alth

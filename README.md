This video is discussing Question 13 of the RHCSA Redhat Exam200, which is related to PodMan.If the video quality is slow, try changing the resolution.
Access All question from this course
https://www.udemy.com/course/redhat-ex200-rhcsa-exam-2024-april-06/?couponCode=KEEPLEARNING

Watch this video to understand the question

https://www.youtube.com/watch?v=pg8P6t9P_3M

<p>This video is discussing Question 13 of the RHCSA Redhat Exam200, which is related to PodMan. If the video quality is slow, try changing the resolution.</p>

<p><a href="https://www.udemy.com/course/redhat-ex200-rhcsa-exam-2024-april-06/?couponCode=KEEPLEARNING">Access All questions from this course</a></p>

<p><a href="https://www.youtube.com/watch?v=pg8P6t9P_3M">Watch this video to understand the question</a></p>

<p><code>useradd alth</code><br>
<code>passwd alth</code><br>
<code>ssh-keygen</code><br>
<code>ssh-copy-id -i /root/.ssh/id_rsa-pub alth@localhost</code><br>
<code>/root/.ssh/id_rsa.pub</code><br>
<code>ssh-copy-id -i /root/.ssh/id_rsa.pub alth@localhost</code><br>
<code>ssh alth@localhost</code></p>

<p><strong>Answer start from here</strong></p>

<p><strong>From root user</strong><br>
<code>Yum install podman* -y</code><br>
<code>systemctl start podman.service</code><br>
<code>systemctl start podman.socket</code><br>
<code>systemctl enable podman.service</code><br>
<code>systemctl enable podman.socket</code><br>
<code>mkdir /opt/file</code><br>
<code>mkdir /opt/outprocess</code><br>
<code>chown alth:alth /opt/files</code><br>
<code>chown alth:alth /opt/processed/</code><br>
<code>ssh alth@localhost</code><br>
<code>podman run -dit --name asciipdf -v /opt/files:/opt/incoming:Z -v /opt/processed:/opt/outgoing:Z monitor</code></p>

<p><code>mkdir -p .config/systemd/user</code><br>
<code>cd ~/.config/systemd/user</code><br>
<code>podman generate systemd --name asciipdf --new --files</code><br>
<code>systemctl --user daemon-reload</code><br>
<code>systemctl --user start container-asciipdf.service</code><br>
<code>systemctl --user enable container-asciipdf.service</code><br>
<code>systemctl --user enable container-asciipdf.service</code><br>
<code>loginctl enable-linger</code><br>
<code>loginctl show-user alth</code></p>


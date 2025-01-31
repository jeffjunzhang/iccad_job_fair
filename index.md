---
layout: default
meta-description: "ACM/IEEE Job Fair at ICCAD. In-person meeting Oct. 31st, 5:30-7:00 pm PT."
---

# ACM SIGDA/IEEE CEDA 2nd Job Fair at ICCAD 2023

**Announcement**:
<!--* We are now having XXX job openings from our company participants!-->
* We are adding an academic job track this year!
* Our in-person meetings are <u> Oct. 31st (Tuesday) 5:30 PM PT </u>! 
  Updated Location: <u> <b> Hyatt Regency San Francisco Downton SoMa (Gallery III)</b></u>. Bring your CVs and enjoy the dinner from ACM SIGDA :) 
* Please [submit your CVs](https://forms.gle/jUk94f874FwiC5og8)  ASAP!

<!--* Join our [email list](https://groups.google.com/) to get notified of the new job openings every week! -->

ACM SIGDA and IEEE CEDA will be holding their annual (2nd) EDA job fair at the [2023 International Conference on Computer-Aided Design (ICCAD)](https://iccad.com) conference, in-person, <b> on Oct 31st (5:30 PM—7:00 PM PST) </b> in San Francisco CA. The job fair is open to all attendees of the ICCAD conference. Attendees are encouraged to submit a CV or résum‌é for circulation beforehand.

The EDA job fair is a place for students and professionals looking for internships or full-time jobs to meet with representatives from companies and academia. At the beginning of the event, one representative from each organization has the opportunity to introduce the organization and its job opening(s). Afterward, all attendees have a chance to mingle.

If you are representing a company, research organization, or university and would like to participate in the job fair, please send an email with your contact information to sigdajobfair@gmail.com. In addition, all job fair participants must [register](https://2023.iccad.com/registration) (for at least one day) for the ICCAD. 
<!--A small participation fee is required (complimentary or discounted participation is available to certain levels of sponsors and exhibitors).-->

<!--
We started live-streaming each talk in this seminar series every week on [YouTube](https://www.youtube.com/channel/UCzz6ructab1U44QPI3HpZEQ)
in the Fall of 2020, and we've been going strong ever since!
Every week we take questions from the live chat and keep videos of the talks
available on YouTube afterward as well.
Give our channel a follow, and tune in every week for an exciting discussion!

Read about our [motivation for starting this seminar](https://hazyresearch.stanford.edu/blog/2020-10-13-mlsys). 

Check out our introductory video:
<iframe width="560" height="315" src="https://www.youtube.com/embed/OEiNnfdxBRE" frameborder="0" allow="accelerometer; autoplay; clipboard-write; encrypted-media; gyroscope; picture-in-picture" allowfullscreen></iframe>
-->

<!-- Read our blog post on our [why we're running this seminar]({{ site.baseurl }}/about). -->

{% for category in site.data.talks %}

# {{ category.type }} 
<div class="talk-list">
  {% for talk in category.members %}
  <div class="talk list-group-item">
  <div class="talk-date">{{ talk.date }}</div>
  <div class="talk-presenter">{{ talk.speaker }}</div>
  {% if talk.title %}
  <div>
    {% if talk.recording %}
      <span><a class="talk-title-link" href="{{ talk.recording }}">{{ talk.title }} <i class="bi bi-box-arrow-up-right"></i></a></span>
    {% elsif talk.livestream %}
      <span><a class="talk-title-link" href="{{ talk.livestream }}">{{ talk.title }} <i class="bi bi-box-arrow-up-right"></i></a></span>
    {% else %}
      <span>{{ talk.title }}</span>
    {% endif %}
  </div>
  {% endif %}
  {% if talk.abstract %}
    <details>
    <summary>Job Openings </summary>
    <ul style="margin-bottom:-30px;">
      {{ talk.abstract }}
    </ul>
      
    {% if talk.bio %}
    <br><br>
    <strong>Mission: </strong> {{ talk.bio }}
    {% endif %}

    {% if talk.recording %}
      <br><br>
      <strong><a href="{{ talk.recording }}">Video Link</a></strong>
    {% elsif talk.livestream %}
      <br><br>
      <strong><a href="{{ talk.livestream }}">Livestream Link</a></strong>
    {% endif %}
    </details>
  {% endif %}
  </div>
  {% endfor %}
</div>
{% endfor %}
*Names in no particular order

# Submit Your CV

As part of the job fair, attendees are encouraged to submit their CV to all of the participating companies before the job fair. This will help companies identify and possibly schedule an onsite interview with you when you attend.

Please clearly indicate on your CV or r‌ésum‌é your availability and type of job interest, along with contact information!

[Upload your CV here to submit to all participating companies.](https://forms.gle/jUk94f874FwiC5og8) 

By uploading your CV, you are agreeing to be contacted by participating and sponsor companies about recruiting and job openings.

# About The Job Fair

**Organizers:** 

Chair, [Vidya Chhabria](https://search.asu.edu/profile/4370240), Assistant Professor, Arizona State University

Co-Chair, [Jeff (Jun) Zhang](https://search.asu.edu/profile/4346755), Assistant Professor, Arizona State University

You can reach us at [sigdajobfair@gmail.com](mailto:sigdajobfair@gmail.com)

**Sponsors:** 

ACM Special Interest Group on Design Automation ([SIGDA](https://www.sigda.org))

IEEE Council on Electronic Design Automation ([CEDA](https://ieee-ceda.org))

International Conference on Computer-Aided Design ([ICCAD](https://iccad.com))


Source code for this website can be found [here](https://github.com/jeffjunzhang/iccad_job_fair).

<!-- Please uncomment this part if you clone our source code! -->
<!--
Website template from the [Stanford MLSys Seminar Series](https://mlsys.stanford.edu).
-->

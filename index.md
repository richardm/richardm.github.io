---
# Feel free to add content and custom Front Matter to this file.
# To modify the layout, see https://jekyllrb.com/docs/themes/#overriding-theme-defaults

layout: home
title: Home
nav_order: 1
---

## Software Engineering Leadership Handbook

{: .quote }

> “The most important thing is that you develop your own principles and ideally write them down, especially if you are working with others.” - Ray Dalio

{: .quote }

> "Everyone makes the mistake of looking at decisions like it's the first problem of this sort... If you have principles, you can learn to think more clearly and communicate better the 'Why'." - Ray Dalio

I started writing down my principles in 2021 after reading [Principles by Ray Dalio](https://www.principles.com/redirect){:target="\_blank"}. These principles are based on a combination of professional experience and extensive reading and are intended to serve as a guide for how engineering leaders should act in common scenarios to optimize their organization. If you have any feedback, disagreement, or suggestions, please open a [GitHub issue](https://github.com/richardm/richardm.github.io/issues){:target="\_blank"} and help me refine these principles.

Since these began as personal notes on my computer, I was not disciplined about noting sources as I encountered ideas. Over time, I will identify and cite sources where possible.

Most of my thoughts here are related to [software development](/software-engineering-best-practices/), [leadership](principles/), [investing](/investing), and [psychology](/psychology). I also have dozens of book notes that I will be sharing as time allows.

<!-- Most ideas are derivative, including these. Share them freely. Principles should be tested and refined. If you have feedback, disagreement, or suggestions, please open a [GitHub issue](https://github.com/richardm/richardm.github.io/issues){:target="\_blank"}. If you take the time to read this, I value your feedback and perspective. -->

{: .wip }

> This is a _very_ rough draft, and I have hundreds more notes to incorporate as I have over time. As a recovering perfectionist, I would prefer to keep this private until perfect, but I am pursuing [progress over perfection](/principles/progress-over-perfection).

{: .critique }

> I have a number of complaints with the current version of this engineering handbook. Enough so that I'm tempted to remove it altogether.
> Some frustrations:
>
> - It presents things as universal absolutes when many of them are contextual. It fails to differentiate clearly.
> - Many of these principles read as pop science rather than explaining the thinking behind them and sharing the real life lessons learned the hard way.
> - It intermixes subjective opinions based on my own personal values rather than presenting universal baseline recommendations based on objective tradeoffs.
> - It provides a lense to how I've approached problems in my past orgs, but that may not apply to how I would approach them in future orgs under different conditions.
>
> Moving Forward:
>
> - I want to develop a rubric explaining common constraints faced by various types of companies: solo founders, early stage startups, mid-sized teams, and mature organizations, and engineering organizations
> - I want to focus on the tradeoffs in light of these business constraints.
> - I want to explained why it makes various recommendations and when these recommendations would not be helpful.
>
> Updating this site has been a low priority for me, but one of these days I plan to overhaul it significantly, because this frankly is not production-worthy.

---

## Who is Richard Morgan?

Unfortunately, having a super generic name like "Richard Morgan" has its challenges from an SEO perspective, and I am working on improving from page 7 in Google for my own name. While browsing for my own site, I discovered some extremely notable and talented Richard Morgans out there.

For disambiguation purposes, I am not:

{% comment %}

<ul>
  {% for person in site.data.richards %}
    <li>{%
        if person.url %}<a href="{{ person.url }}" target="_blank" rel="nofollow">{{ person.title }}</a>{% else %}{{ person.title }}{% endif
      %}{%
        if person.note %}<span class="mx-0 px-0">({{person.note}})</span>{% endif
      %}</li>
  {% endfor %}
</ul>
{% endcomment %}

---

- [Richard K. Morgan, the author](https://www.richardkmorgan.com/){:target="\_blank" rel="nofollow"}
- [Richard Morgan†, the 9/11 First Responder](https://www.911memorial.org/connect/blog/honoring-life-911-first-responder-richard-morgan){:target="\_blank" rel="nofollow"} (but you should read his memorial)
- [Richard A. Morgan, the Comic artist](https://www.instagram.com/richardamorgan/){:target="\_blank" rel="nofollow"}
- [Richard J. Morgan, the journalist and writer who lives in Paris](http://charmandrigor.com/){:target="\_blank" rel="nofollow"} (he should enable SSL)
- [Richard C. Morgan, the spine care physician in Miami, Florida](https://baptisthealth.net/doctors/richard-colin-morgan/2611627){:target="\_blank" rel="nofollow"}
- [Richard Morgan, the men's basketball coach in Virginia](https://burams.com/news/2025/3/3/athletic-dept-richard-morgan-steps-down-as-bluefield-university-mens-basketball-coach.aspx){:target="\_blank" rel="nofollow"}
- [Richard Morgan, the estate planning attorney in Georgia](https://morgandisalvo.com/people/richard-morgan/){:target="\_blank" rel="nofollow"}
- [Richard Morgan, the BBC journalist in Belfast](https://x.com/bbcrichardm){:target="\_blank" rel="nofollow"}
- [Richard G. Morgan, the trial attorney in Minnesota](https://www.huschblackwell.com/professionals/richard-morgan){:target="\_blank" rel="nofollow"}
- [Richard Morgan, Ph.D., MSW, the clinical professor at Stony Brook](https://socialwelfare.stonybrookmedicine.edu/faculty-staff/morgan){:target="\_blank" rel="nofollow"}
- [Richard Morgan†, the 92 year old four-time rowing world champion](https://www.rte.ie/brainstorm/2025/0218/1497376-richard-morgan-92-year-old-rowing-world-championships-fitness-health-older-adults/){:target="\_blank" rel="nofollow"}
- [Richard Morgan, house staff at Duke Ophthalmology](https://dukeeyecenter.duke.edu/profile/richard-morgan){:target="\_blank" rel="nofollow"}
- [Professor Richard Morgan, the Director of the Centre for Hypersonics at the University of Queensland](https://about.uq.edu.au/experts/256){:target="\_blank" rel="nofollow"}
- [Professor Richard Morgan, Dean of Biosciences, Professor of Molecular Oncology at the University of West London](https://www.uwl.ac.uk/staff/richard-morgan){:target="\_blank" rel="nofollow"}
- [Dr. Richard Morgan, the assistant professor at Durham University Business School](https://www.durham.ac.uk/business/our-people/r-h-morgan/){:target="\_blank" rel="nofollow"}
- [Richard Morgan KC, the barrister at Maitland Chambers](https://www.maitlandchambers.com/our-people/profile/richard-morgan-kc){:target="\_blank" rel="nofollow"}
- [Richard Morgan, the golf coach in Alabama](https://calhoun.edu/directory/richard-morgan/){:target="\_blank" rel="nofollow"}
- [Richard Morgan, the Australian actor](https://www.themoviedb.org/person/137351-richard-morgan){:target="\_blank" rel="nofollow"}
- [Richard Eugene Morgan†, the former mayor of Gillette, Wyoming](https://www.gillettenewsrecord.com/obituaries/article_fd794505-369b-4258-a906-c60c8cbcd321.html){:target="\_blank" rel="nofollow"}
- [Morgan Richard Olivier, the author in Louisiana](https://morganrichardolivier.com/){:target="\_blank" rel="nofollow"}

![commits](https://badgen.net/github/commits/richardm/richardm.github.io/main?cache=300) ![last commit](https://badgen.net/github/last-commit/richardm/richardm.github.io/main?cache=300)

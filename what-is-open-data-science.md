
This is a summary of a private conversation that has append following what's
look like a relatively simple [an harmless
PR](https://github.com/jupyter/jupyter/pull/21) on the Jupyter project, that
lead us to the realisation that we didn't had a clear distinction in between
or formal goal and informal behavior in what we accept an reject.

The title of the above Pull request was pretty simple and self explanatory:

> Add MATLAB kernel to data_science.rst documentation

So before you head to the PR to see wether we merged it or not, 
what would you have done ?

In the following paragraphs we investigate a few thougths on that.


# Can we legally do it ?

> I think that is fine but we would probably have to add the "MATLAB is
a Trademark of ..." language to the page.

# We promote Open science.

> The whole goal of that page was to provide a biased and
> not-entirely-fair place to promote our vision of Jupyter in the data
> science space. To me, that page is about promoting, in a marketing
> focused way, the most popular open source and (yes) hyped kernels for
> data science. The O'Reilly Data Science Survey is a great source to
> see what tools are popular in Data Science. Python and R are right at
> the very top of the list. Matlab is present, but near the bottom of
> the list (JavaScript is used by ~2x the number of people at Matlab in
> data science, why not list it?). It is also commercial, and doesn't
> really fit well ideologically in our traditional vision of data
> science and science. So I guess I am -1 on listing Matlab on that
> page.

> http://www.oreilly.com/data/free/2014-data-science-salary-survey.csp



# We don't descriminate

> Why don't we instead put a link at the bottom to our full list of kernels, and rewrite the text to say "Here are some of the most highly-used open-source languages for data science."



> 1 my personal perspective: I am strongly in favor of the project having a clear open source mission statement.  Our BSD licensing makes it clear that building proprietary tools is *possible*, and that we have a great story interoperating with industry, but we are first and foremost an open source, open science project.

> 2 personal ideas aside, we are legally part of Numfocus, which has a fiduciary responsibility with the IRS to uphold ideas of open source and open science for the public good, in return for its tax exempt status.  This is the one place were we DO give up some independence in return for the benefits that Numfocus provides to us as a Fiscal Sponsor: IPython/Jupyter is legally an *agent* of Numfocus, and must therefore act in conformance with the charter of Numfocus.


# We do promote and use Proprietary tools

>I agree with everything Fernando said, but at the same time, we do
>promote some non-open source software at times - GitHub, Plotly,
>Anaconda are examples. I am not sure we want to make the case for
>non-inclusion of Matlab on this page in such philosophical terms, lest
>we paint ourselves into a situation where we do want to include
>commercial software in our messaging and end up contradicting our own
>statements.
>
>To me, the main point of the data science page is not to make a
>philosophical statement about open-source software, but to "market"
>our software to data scientists. In the context of that page, the fact
>that our software is open-source serves the greater goal of the page,
>not the opposite. The greater goal of the page might even lead us to
>promote promote third party, commercial sites, such as GitHub,
>Microsoft Azure or O'Reilly that have excellent integration with our
>tools related to data science.
>
>Put another way: open-source is a means to a much greater end that
>sometimes requires us to partner with and promote non-open source
>software. Without these greater goals, it is hard to understand why we
>would collaborate with and promote commercial companies like GitHub.
>
>I do think it is important for us to acknowledge our collaborations
>and funding from these (and other) companies and the bias that it
>creates.
>
>I also think that this is exactly the type of thing that the Steering
>Council should discuss and decide.
>
>

>Excellent points indeed, and I think it's important that we do clarify these...
>
>From my perspective, it boils down to the question: is a tool "on the critical path" of a scientific result, or at least in principle "incidental" to the result itself?  If the former, I'm pretty much Stallman-esque in that it MUST be open, full-stop, as a matter of principle.  
>
>Just like a theorem whose proof I'm not allowed to read is not mathematics, I don't want scientific results built upon toolchains that I can't either open up or tell students that they are legally prevented from studying.
>
>If the latter, it's a different story: while I think github makes us vastly, astronomically more effective as a community, we could all in principle collaborate on academically-hosted repos running gitlab from our universities, for example, if Github went 'all evil'.  OpenStack, for all its troubles, does offer us at least the promise of a plan B to run self-hosted cloud stacks if we want to move away from Amazon/Azure/etc...  While Anaconda may offer us the convenience of easy installers, Continuum has been a solid community player in fully open sourcing the conda code itself, so while there's a real loss of convenience in the packages and recipes behind Anaconda, if they also go 'all evil', it's not inconceivable to fund the effort for a viable alternative.
>
>For each of these, a 'plan B' is actually reasonable, and they also don't sit in the intellectual critical path, they right now provide infrastructure that mostly makes our lives easier.  Easier in immensely important ways (as in, often the difference between impossible and possible), but still, I think there's a real difference between that and having the core Matlab or Mathematica code being close-source and having that be the code behind an entire scientific community (as is the case in some fields).
>
>
>I put this out, in the hope that it helps...  We'll need to find a good way to present a consistent perspective that includes all these nuances.
>


> I do think the "introspectability" of open source code is critically
> important for open, reproducible science. But I have found that many
> users just don't quite buy that. I hear things like "sure maybe in
> principle that is important, but in practice I have never needed to
> look at IPython/Matlab/Mathematica's source code to reproduce or
> understand research" While I can surely imagine situations where one
> would need/want to look at the details of a numerical algorithm, it is
> hard to see how that same need extends to the user interfaces
> themselves.
> 
> To me, I think there is another argument for the importance of open
> source in science that is more convincing, and which also clarifies
> why some commercial services/software like GitHub are an important
> part of the picture. My argument is that there should be as few
> barriers as possible for others to reproduce the results of research.
> What types of barriers get in the way?
> 
> * Expensive, proprietary software (Matlab/Mathematica) that few can afford.
> * Closed journals that only wealthy, first world universities can afford.
> * Poor software engineering practices (no tests, no/bad documentation,
> no versions control).
> * Software with no collaboration features.
> * Poor usability and design of software.
> * ...and the list goes on...
> 
> Software that is open-source, usable, well designed, free, documented,
> collaborative, version controlled makes it easier to do and reproduce
> research. But the "open-source" quality of this software is just one
> of the many characteristics that reduces the barriers. Given the
> ongoing socioeconomic injustice that is still present in our world, I
> think it is especially important as it opens the scientific method and
> results to underrepresented, disadvantaged and even oppressed groups
> of people. Put another way: high-quality open source software is an
> important part of the battle against "science done by and available
> only to rich white men." That is of deep societal and ethical
> importance.
> 
> From this perspective, the desirability of GitHub is clear: it further
> reduces the barriers for people to share code+data and brings this to
> literally *everyone* (not just well off people who can afford to run
> their own git servers). I like this way of thinking as it provide a
> simple criteria for evaluating tools: does it reduce the barriers and
> open participation to more people?

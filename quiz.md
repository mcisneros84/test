# Question 1

You receive the following ticket from a customer:

> Hi GitHub!
> So according to the docs at https://developer.github.com/v3/orgs/teams/#add-team-repo, I should be able to add teams to a repo programmatically.
>
> However, this does not work when using the following code:
>
> curl -H "Authorization: token BLAHBLAHBLAH" -H "Content-Length: 0" -X put -d "" https://hostname/api/v3/teams/23/repos/jimmy/some-repo-name
>-
> Could someone give me a curl one liner that lets me add teams to repos ? Or at least tell me what facet of the documentation has escaped me for the last 45 minutes?

Notes:
Be sure to include an example curl command that will work in the customer response.

# Response 1

Hi ‘Customer’ (where customer is the actual name)

Thank you for contacting GitHub. My name is Martha and I will be assisting you.  

As you have read, the repository must be owned by your organization, or a direct fork of a repository owned by it.  I’m very sorry if we missed something in our documentation that didn’t make clear that /:org/ was the attribute for the organization that owns the repository. With that being said, please try this code:

> curl -H "Authorization: token BLAHBLAHBLAH" -H "Content-Length: 0" -X put -d "" https://hostname/api/v3/teams/23/repos/org-name/some-repo-name

Please let me know how it goes and do not hesitate on contacting me with any more questions or comments regarding this issue.

Regards,

Martha

# Question 2

You receive a ticket from ACME, Inc. asking if it's possible to adjust GitHub Enterprise's web-interface to match their corporate identity better.

> Hi,
> At ACME, Inc. we have many services running in-house, all matching our orange colored corporate design and showing the ACME, Inc. logo. GitHub Enterprise is the only service that does not seem to support this. How can we alter GitHub Enterprise's design?

GitHub currently does not support modifications to GitHub Enterprise's web-interface for two reasons:

* GitHub Enterprise was designed to match GitHub.com to preserve the familiarity many software developers around the world have already acquired on GitHub.com. Changing the GitHub user experience by altering its design could be too confusing for the people actually using our product.
* Changing GitHub Enterprise's design would only be a cosmetic change. It wouldn't have a huge impact on improving how people collaborate and work together as other features we could be working on. There are other items on our product's roadmap with a higher prioritization.

# Response 2

Hello ‘Customer’

Thank you for contacting GitHub Enterprise.  We understand the importance of branding your in-house services with your corporate design and thank you for bringing that into our attention. 

GitHub Enterprise was designed to match GitHub.com to provide the best end-user experience as possible, by ensuring your engineers receive continuity and minimize the confussion in between products.

It’s on our best interest to guarantee your business continuity and satisfaction, and if you truly believe that this cosmetic change would have a great impact on  the way people collaborate in your organization while using GitHub Enterprise I would escalate this to my next level, as for now, our Engineering department is working in other items that will improve the experience and functionality of the whole product.

Regards, 

# Question 3

You receive the following ticket from a customer:

> Hi!
>
> After installing the latest update this morning I noticed that my browsers are now throwing Invalid SSL Cert errors when attempting to access our instance.
>
> $ curl -I https://github.acme.edu
> curl: (60) SSL certificate problem, verify that the CA cert is OK. Details:
> error:14090086:SSL routines:SSL3_GET_SERVER_CERTIFICATE:certificate verify failed
> More details here: http://curl.haxx.se/docs/sslcerts.html
>
> Not sure if anyone else has reported this or what I might be able to do to fix it. I've re-uploaded our key & cert file to no avail.

Notes

You do not have shell or web interface access to their GitHub Enterprise instance, so in your reply you'll need to have the customer do any troubleshooting steps and return the results.

# Response 3



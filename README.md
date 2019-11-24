# Beta Books

## Overview

A site for authors and beta readers to create better books together.

## Notes

### 24-Nov-2019 - A General Braindump, Presaging The Shape of Things to Come

The premise of beta-my-book is that, as an author, I would like to be able to share a book I'm in the process of writing and editing with a select set of beta readers who can comment in real-time. I imagine it being like a git pull request for coders. The author puts up draft work for review. The readers review it and make comments both inline and in general. Some comments are suggested edits (ie, for typos) while others are more general feedback.

**Users, objects, and stuff**: The core functionality of an MVP: 

Authors can login and start creating a story. There is a basic rich-text editor and a backing store. Imports from other formats will probably need to be an early feature. Proper name detection and "story helpers" would come later. Export to e-publishing formats is an obvious requirement ultimately. Possibly monetize by linking to the third-party tools needed to make a book presentable for ePub (cover designers, et alia.)

Near-constant autosave and the ability to review and rewind to a previous point in time are essential. While the author is working on a chapter, (or other subpart of the book as they see fit. Mark by section as a later option?) it's stored as draft. Once they're ready to get feedback, they release (publish?) to their beta readers.

Authors can request and send out "beta-reader invite links." These invite a potential reader to beta a specific work or everything a writer is working on. Beta readers can sign up via the link. Once a reader is in the system, they should have a single identity for all the works they're reviewing across authors.

**The front page**: When unauthorized users come to the site, they should see an explanation of the site's purpose, a news stream, a way to find works looking for beta readers, a means to sign up as an author and a means to sign up to be kept up-to-date with site happenings including the availability of new works by genre/subject/author to review. Links to more detailed information and possibly things to buy should also be available.

#### Big questions to answer

* Is it viable to architect this as a static site with Azure functions on the back-end? I still haven't seen a clean implementation of Azure functions to Azure SQL.
* Specifically, how practical is it to manage auth(orization|entication) via FaaS?
* Does it make sense to use git to store the actual works? It would handle a lot of the diff-patch-merge work for me, but it's not a well-established tech path.
* How much is this going to cost to run? How can I make it pay for itself?
* Do I want to use an existing CSS framework or design it myself?
* What other technologies do I want to use?
* Do I want to outsource any part of this?
* How do I find what features people will actually want to use?
* Domain name?
* How do I want to deploy this?
* E-mail alerts? MailChimp? SendMail?
* Explicitness slider on user preferences?
* Requirements of legal representation as a content host?
* Do I blog about building this?
* Live chat feature?
* Collaboration between authors?

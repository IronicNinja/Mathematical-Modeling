# HiMCM 2020 Problem B Finalist Paper (Top 7%)

If you would like to access the notebook and test out our solution, click here: https://colab.research.google.com/drive/1thAS-eMqCOOi0IfcC-jmwDxht6eNs7xU

### From our Summary Sheet

This paper focuses on devising an algorithm to create an optimal funding schedule so that the FRPCE is able to acquire the “long term and reliable” funding necessary to complete all 48 conservation projects within a reasonable timeframe. First, we identify the objectives that the FRPCE should consider when making budget decisions. We also identify the characteristics of imperiled species that should be considered by the board in determining the schedule. 

With this information, we split our plan into two sections. The first section is 5 years long and consists of an initial portfolio with short projects that are highly beneficial to the environment and are very likely to succeed. By having a strong initial portfolio of projects, the board is able to signal to potential donors, grantors, or investors that there is a strong sense of direction and organization when completing these conservation projects. Investors then would be more inclined to provide “long term and reliable” funding to complete the remaining projects. In our initial portfolio, we also include the two projects that have a taxonomic uniqueness value of 1.00, as those are the projects that are most at risk for extinction. Using a Python script, we calculate all possible configurations of the initial portfolio and then choose the configuration that has the lowest standard deviation of 5-year costs, effectively allowing the board to raise funds consistently.

Our second section is 24 years long and consists of the remaining 38 conservation projects. Our plan ensures the board will receive adequate funding every year by minimizing the chance that the majority of projects fail in one year, as investors would be less inclined to fund our projects if there was a year where multiple projects failed. We minimize this chance by maximizing the feasibility one project will succeed every year by pairing high feasibility projects with low feasibility projects. By doing so, we achieve a consistent average that maximizes our success. We advise that the board does not end more than one pair of projects in the same year to maximize the positive yield of our projects and to avoid congregating costs into a short period of time.

With the pairs set in place, we utilize a greedy algorithm to prioritize the pairs that have the highest expected benefit. Using a Python script, we organized the 19 pairs of projects into a span of 25 years, finalizing our schedule for the 48 conservation projects. We then introduce a fundraising strategy that involves investing some amount of the fundraised money into an endowment to reduce the total amount of money that needs to be raised through traditional fundraising.

Overall, our solution will allow the board to achieve “long term and reliable” funding by accounting for investors’ intentions and investing efficiently.

Credits to Daniel Jin, Trey Wiedmann, and Daniel Xie for helping complete the project as Team #11318.

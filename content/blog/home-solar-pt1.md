+++
title = "Home Solar, Part 1: Introduction"
date = 2024-10-27
description = "Installing a solar system at home, part 1: introduction"
authors = ["Andrew Dunham"]

[taxonomies]
categories = ["House", "Tech"]
tags = ["house", "projects", "solar"]

[extra]
lang = "en"
toc = true
+++

We've just finished a long-running project to install solar panels on our
house. This is the first of a series of posts about the project, where we aim
to cover everything from the initial planning to the final installation,
along with posts on ongoing monitoring, troubleshooting, and lessons learned.

<!-- more -->

## Why Solar?

We've been thinking about installing a solar system for a while, for a few
reasons, and the combination of these reasons and having some time in our lives
for projects meant that it made sense for us to do it at the time.
Additionally, the cost of solar panels had come down significantly at the time
we began the project.

### Electrification

We care about electrification and green energy, and reducing our usage of
fossil fuels. We've been slowly replacing all of our fossil-fuel powered
appliances with electrified versions (induction stove, electric hot water
heater, etc.), so more of our utility costs are electrical vs. from natural
gas. We also drive an EV, so being able to charge our car with solar power for
a good part of the year is a bonus.

### Power Outages and Resilience

We live in an area with semi-frequent power outages, and we wanted to have a
system that could keep the lights on and the sump pump running during an
outage. We'd previously put a generator in, but in May 2022 we experienced a
power outage that lasted for more than a week, and home standby generators are
not designed to run continuously for that long. Additionally, the cost of
natural gas for that week was several hundred dollars, along with the
maintenance costs of the generator, new spark plugs, oil changes, etc.

Our house has a sump pump that keeps water out of our basement, and in a very
heavy rainstorm (or the spring melt), we measured the inflow into our sump pit
to be on the order of 1L/second of water. At this rate, if the power goes out
and our sump pump stopped pumping, we'd have less than 15 minutes before our
basement floods. We also have a backup sump pump, but it's not as powerful as
the main one, and it's insufficient to keep up with the inflow; it buys us an
hour or two, but it's not enough to prevent a flood.

### Electricity Bill Reduction

We wanted to save money on our electricity bill, and the current rules for net
metering in Ontario are quite favorable to households with rooftop solar.
Specifically, any power that you export to the power grid is credited at the
same rate as the power you import, and you can carry over credits from one
month to the next. This means that you can effectively "store" power in the
grid for use in the winter, when your solar panels are producing less power.

Additionally, [a recent ruling][oeb-ruling] by the Ontario Energy Board
required power companies to allow customers that were on a time-of-use plan to
use net metering, instead of the previous behaviour where customers were forced
to transition to a tiered plan. Since most time-of-use plans charge a higher
rate for power during the middle day, when the sun is shining, you're getting
more value for your solar export.

[oeb-ruling]: https://www.hydroone.com/businessservices_/generators_/Documents/OEBStaff-Bulletin-TOU-Option-for-Net-Metered-Customers-20230117.pdf

## Initial Planning

When we were planning out our installation, we had a few key principles in
mind, that we'll cover here:

1. **High Reliability:** We wanted a system that was reliable, with a good
   track record for long-term operation. This means that we weren't interested
   in no-name or re-branded cheaper OEM equipment, and we were willing to pay a
   bit more for a system from a larger brand.
2. **No Proprietary Systems:** We wanted to, as much as possible, avoid
   proprietary systems that would lock us into a single vendor for the life of
   the system. This means that we avoided systems like Tesla's Powerwall, and
   instead went with a system that was more modular and could be expanded or
   replaced in the future. Since we knew that we wanted to add battery storage
   after the initial solar installation, we wanted to make sure that the system
   we chose would be compatible with a variety of batteries (more on this
   below).
3. **Minimal Single Points of Failure:** We wanted to avoid having a single
   point of failure that would take down the entire system. While we ended up
   compromising somewhat on this particular point, we did our best to minimize
   the number of things that could go wrong and take down the entire system.

   Additionally, we wanted to make sure that if a single component failed, we
   had the ability to bypass it such that the rest of the house wouldn't be
   left without power.
4. **No Cloud/Internet:** We didn't want a system that required an internet
   connection to operate, or that required a cloud service to function. In
   addition to the fact that we've been dealing with a flaky internet
   connection at home, both of us work in infosec and have a general distrust
   of cloud services.
5. **Easy to Monitor and Troubleshoot:** We wanted a system that was easy to
   monitor and troubleshoot, and that could be integrated into Home Assistant.
   More on this in a later post in this series.
6. **Scalable for Future Expansion:** We wanted a system that could be easily
   expanded in the future, for example, if we wanted to add more solar panels
   or a battery system. Since we have future plans to re-do our garage and
   weren't installing solar panels there, we intentionally sized our system to
   be large enough so that we could add more panels in the future without
   needing to buy a new inverter.
7. **Battery Storage:** We knew that we wanted to add battery storage to our
   system, even though we weren't planning on doing it at the same time as we
   installed solar panels. This meant that we needed to choose an inverter that
   was compatible with a variety of battery systems (see the "no proprietary
   systems" point), and that we needed to plan for the eventual addition of
   batteries. More on this in a later post in this series.
8. **100% Code Compliance:** We wanted to make sure that our system was 100%
   code compliant, which meant installing equipment certified for use in
   Ontario and ensuring that all necessary notifications and inspections were
   filed and completed. While it is technically possible to DIY such an
   installation in Ontario, it's a fair bit of work and we wanted to make sure
   that everything was done correctly, so we worked with a reputable local
   installer.

We used these principles to guide our decision-making process, and we'll
explain more on this in a later post where we cover the equipment we chose and
how the equipment met these principles.

### Financial Planning

In addition to the principles behind our system, we also made an explicit
choice to go with a "large" system–specifically, one that made full use of the
south-facing roof of our (modestly-sized) house. This is very much a decision
that's specific to the financial situation of every household, but in our case
we're fortunate enough that we were able to make that choice.

Depending on your financial situation, you might choose to install a smaller
system with room for expansion, or apply for grants or loans.

In general, if you don't care about specific equipment and just want to reduce
your electricity bill, the best way to do that is to get multiple quotes from
reputable installers and choose the quote with the lowest cost in terms of
dollars per watt of solar panels actually installed, ignoring any grants or
rebates. Make sure that you're comparing apples to apples here; don't compare
using the theoretical capacity of an inverter. Comparing the actual wattage of
installed solar panels is comparing the theoretical maximum output of the
system across all quotes.

Of course, make sure that you trust the installer; they're responsible for any
warranty work, so they need to be reliable enough to be around in a few years
when you need them!

The cost calculations for batteries are substantially more complex, and we'll
cover that in a later post in this series.

{% note() %}
Some installers will give you a "payback period" for your system, which
typically includes a lot of assumptions about future electricity prices,
whether net metering will continue to exist in its current form, and so on.

It's worth running your own numbers to see what the payback period is for your
system, and playing around with the assumptions to see what happens in a
variety of scenarios. However, broadly speaking, most solar equipment comes
with a warranty of at least 10 years. So, if your payback period is less than 7
years, you're in a great situation and should almost certainly move ahead. If
it's between 7-10 years, it's a good investment, but you should probably
double-check any assumptions. If it's more than 10 years, you should be careful
to temper your expectations regarding the financial return.

Additionally, these "payback periods" typically don't include a comparison to
just putting the money you'd spend in an investment, so if you're solely
motivated by financial return, you should consider that as well.
{% end %}

## Up Next

In the [next part](@/blog/home-solar-pt2.md) of this series, we'll cover some
terms and definitions that you might encounter while doing a solar installation
in Ontario (or elsewhere).  Stay tuned!

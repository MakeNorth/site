+++
title = "Home Solar, Part 2: Definitions and Terms"
date = 2024-10-28
description = "Installing a solar system at home, part 1: definitions and terms"
authors = ["Andrew Dunham"]

[taxonomies]
categories = ["House", "Tech"]
tags = ["house", "projects", "solar"]

[extra]
lang = "en"
toc = true
+++

This blog post is the second in a series about installing solar panels on our
house. In this post, we'll go over many of the definitions and terms that we
came across, and try to define them in a way that's useful for someone that's
not an electrician or solar installer.

<!-- more -->

## Definitions

While we were planning our installation, we came across a lot of terms that
and definitions, which we cover here to help you understand the rest of the
series. We assume that you have a basic understanding of electrical terminology
like AC vs. DC, volts, amps, watts, etc.

While many of the terms here are general and helpful when thinking about solar
installations anywhere, some of them are specific to Ontario or Ottawa, where
we live.

{% tip() %}
This post is pretty dense, and you don't need to read and understand all of it
to get started with a solar installation. If you're just getting started, you
can probably skip this post and refer back to it later. Feel free to jump ahead!
{% end %}

{% warning() %}
We're not electricians, and–despite having learned a lot during the course of
this project–we're not experts in solar installations. This section is based on
our understanding of the terms and concepts, and we're not responsible for any
errors or omissions. If you're planning on installing a solar system, you
should consult with a professional installer, electrician, and/or engineer.

If you notice anything that's incorrect or missing, please
[let us know](/about/) so we can correct it.
{% end %}

### Components and Hardware

- **Solar panels**, sometimes called photovoltaic panels, or PV, are the
  components of the system that actually produce power. They have a variety of
  properties that are important when designing a system, and we'll cover more
  about them in a later post.
- **Optimizers/rapid shutdown devices** are devices that attach to a solar
  panel (or are integrated into the panel) that are used when not using a
  microinverter-based system. Per code in Ontario, all solar systems must have
  a so-called "rapid shutdown", sometimes abbreviated RSD, that allows the
  system to be shut down in case of a fire or other emergency. Some RSDs also
  have the ability to optimize the power output at a per-panel level to reduce
  the impact of shade. Microinverters will provide rapid shutdown functionality
  when those are being used, and thus a separate device is not required.
- **Inverter** is the component that converts the DC power produced by the
  solar panels (or batteries) into AC power that can be used by your house, or
  exported to the rest of the power grid.
    - For inverters that support battery storage, they can typically also
      charge the battery by drawing AC power from the grid. These are sometimes
      called "inverter-chargers".
    - There are two major types of inverters in use in residential
      installations today: microinverters vs. string inverters. We'll go into
      more detail in a later post, but broadly speaking, a microinverter is a
      small inverter that attaches to a single solar panel (or sometimes 2/4
      panels), while a string inverter is a larger inverter that attaches to
      multiple panels that are connected in series in a "string".
- **Batteries** are the component(s) that stores power for use later. There are
  a variety of battery chemistries in use today, and we'll cover more about
  them in a later post. Broadly speaking, though, there are two types of
  battery systems:
    - AC-coupled batteries (like the Tesla Powerwall) are connected to other
      components of the system and the power grid via an AC connection, and
      integrate an inverter-charger into the battery itself.
    - DC-coupled batteries (similar to a lead-acid or AGM battery that you'd
      find in your car) are connected to the rest of the system via a DC
      connection, and require a separate inverter to convert the DC power to AC
      power and vice-versa. So-called "all-in-one" inverters typically provide
      both the DC-AC conversion to connect solar panels and the DC-to-AC or
      AC-to-DC conversion for a connected battery.
- **Balance of system** refers to all the other components of the system that
  aren't the solar panels, inverters, or batteries. This includes things like
  wiring, fuses, breakers, junction boxes, disconnects, and so on.
- **Lamacoids** are the labels that are required to be placed on certain
  components of the system, to either provide information about the component
  or system (e.g. a copy of the SLD, described below) or to display a warning,
  such as "Two Power Sources" or "Rapid Shutdown Switch".

  The word "lamacoid" is a trade name; the generic term for these is
  "nameplate", "legend plate", or "engraved plate". Typically, they are
  required to be weatherproof.

### Parties

- A **Solar Installer** is the company that installs the solar system. They're
  responsible for the design, permitting, installation, and commissioning of
  the system. They're also responsible for interfacing with the electrical
  utility and the Electrical Safety Authority (ESA) to get the necessary
  permits and inspections. They typically also provide a post-installation
  warranty and are responsible for any maintenance or troubleshooting that may
  be required.
- **Electrical Safety Authority** (ESA) is the organization that is responsible
  for electrical safety in Ontario. They must be notified before any work is
  done, and will perform inspections and ensure that all electrical work is
  done to code.
- The **Electrical Utility** is the company that provides power to your house.
  They're responsible for the power grid, billing, and are the final arbiter of
  whether a solar installation can be connected to the power grid, and how
  large of an installation is allowed. Sometimes referred to as the "power
  utility", "power company", "hydro company", etc. Here in Ottawa, this is
  [Hydro Ottawa][hydro-ottawa]; elsewhere in Ontario it's typically
  [Hydro One][hydro-one].

  The phrase "supply authority" (e.g. as used by the ESA) can refer to the
  electrical utility as well, though it's more general than just the utility.
- A **Professional Engineer** (abbreviated P.Eng.) is a person who is licensed
  to practice engineering in the province of Ontario. Note that this is
  different from someone that has a degree in engineering; a P.Eng. is a person
  who has passed the professional engineering exam and has been granted a
  license by Professional Engineers Ontario. Certain aspects of the solar
  installation must be designed and stamped by a professional engineer.
- A **Master Electrician** is a person who is licensed to perform electrical
  work in the province of Ontario, by passing the master electrician exam
  administered by the ESA. They are responsible for the installation of the
  electrical components of the solar system, and are typically employed by the
  solar installer.
- A **Licensed Electrical Contractor** is a company that is allowed to perform
  electrical work in the province of Ontario. They employ electricians to
  perform the work.

{% note() %}
A professional engineer is very different from an electrician; an engineer is
responsible for the design of the system, while an electrician is responsible
for the installation. Unless a P.Eng. is also a licensed electrician, they
cannot perform the installation themselves. Unless a licensed electrician is
also a P.Eng., they cannot design a system that requires a P.Eng. stamp.
{% end %}

[hydro-ottawa]: https://hydroottawa.com/
[hydro-one]: https://www.hydroone.com/

### Planning, Design, and Permits

- **Single-line diagram** (sometimes abbreviated as "SLD") is a diagram that
  shows the electrical connections between all the components of the system.
  This is a required document for the permit application and interconnection
  agreements with the electrical utility, and it's also a useful document to
  have when troubleshooting the system.
- **Permit**, despite being a common term, is a bit of a misnomer in Ontario.
  To use the official terminology; you file a "notification of work" with the
  Electrical Safety Authority (ESA), where you specify the scope of the work
  that you're intending to do. The fees for these notifications are fairly
  complicated, but the ESA will walk you through the process on the phone. This
  is typically done by the solar installer.
- **Inspections** are the process whereby an inspector from the ESA will come
  out to your house and inspect the work that was done. This is typically
  scheduled by the solar installer, and the inspector will check that the work
  was done to code and that it's safe. In Ontario, there are two kinds of
  inspections:
    - **Rough-in inspections** are done before the system is energized, and
      checks that the wiring is done correctly, safety requirements are met,
      only approved components are used, etc. This inspection must be completed
      before the system is energized, and before any of the work completed is
      covered up (e.g. by drywall).
    - **Final inspections** are done after the system is completed, and must
      performed before the electrical utility will grant permission to connect
      to and feed power back to the grid. Upon completion of the final
      inspection, the ESA will issue a **Certificate of Inspection** that the
      utility will require a copy of.
- **Connection Authorization** is an approval from the ESA that the system is
  safe to connect to the power grid. This is typically required by the
  electrical utility before they will allow the system to be connected. The ESA
  will issue a "Connection Authorization Verification" certificate.
- **Distributed Energy Resources**, often abbreviated "DER", is the term used
  by the electrical utility to refer to solar systems, battery storage, and
  other small-scale power generation systems. In Ontario, if your generation is
  a so-called "micro-generation" project, consisting of less than 10kW AC worth
  of generation capacity, then typically the utility will perform an
  abbreviated review of the system on a relatively short timeline and with
  minimal fees.

{% important() %}
The electrical utility cares about the so-called "nameplate capacity" of any
power generation, not what is theoretically possible in a given installation.
So hypothetically, if you install a 20kW inverter, but only 8kW of solar
panels, the utility will consider your system to be 20kW, and you'll be
ineligible for the micro-generation program, even though your system is
incapable of generating more than 8kW of power.
{% end %}

- **Connection Impact Assessment** (often abbreviated "CIA") is the name of a
  form that must be filled out and submitted to the electrical utility. This
  form is used by the utility to determine if the proposed solar system will
  have any impact on the grid, and if there is capacity to support the proposed
  amount of power generation. This form is typically filled out by the solar
  installer, and is typically not required for micro-generation projects under
  10kW AC of generation capacity.

  Another name for this is a "Distribution Connection Impact Assessment"
  (abbreviated DCIA).

{% note() %}
At least for Hydro Ottawa, the CIA application and drawings need to be stamped and
signed by a professional engineer who is licensed in the province of Ontario
and in good standing; this is a requirement regardless of who is performing the
installation.
{% end %}

{% important() %}
The timeline for a CIA can be quite long, especially if the utility has to
perform a detailed review of the system, or if they're backlogged with
applications. In our case, the CIA was submitted on October 6, 2022 and was
approved on November 29, 2022, but we've heard anecdotal reports of the process
taking many months.
{% end %}

- An **Electrical Operation and Maintenance Agreement** (abbreviated EOMA) is a
  document that is signed by the homeowner and the electrical utility, that
  specifies the responsibilities of each. In our case (with Hydro Ottawa), this
  document specifies a collection of requirements, but more relevant to us,
  also include direct contact information for both the homeowner and the local
  system operator, in case either party needs to contact the other. While this
  hasn't come up so far from us, the agreement also states:

{% quote(cite="Hydro Ottawa EOMA") %}
Each party’s Controlling Authority shall be available to each other on a 24/7
basis. Unavailability of the Customer’s Controlling Authority may result in
Hydro Ottawa’s Controlling Authority disconnecting the DER.
{% end %}

- **Generation Connection Agreement** (GCA) is another agreement that we signed
  with Hydro Ottawa.


### Other Terms

- **Distributed Generation** is the generic term used to refer to power
  generators that are connected to a distribution system.

- **Home-Run** is a term used to refer to a run of electrical cable that goes
  directly from a single component to a central location, rather than daisy
  chaining components together. This is typically used to refer to the wiring
  from the end of a string of solar panels back to the inverter; panels are
  typically connected such that the positives are all in series,
  positive-to-negative, and then the final ends are connected to the inverter.

## Up Next

In the next part of this series, we'll cover how we found and chose our solar
installer, and how we picked the specific components of our system. Stay tuned!

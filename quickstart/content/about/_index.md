+++
date = "2018-09-02"
draft = false
title = "About Me"

+++

Hello! My name is Anna Liao. I am currently a DevOps SysAdmin for an OpenStack cloud at [Cybera](http://www.cybera.ca/), a non-profit [research and education network](https://en.wikipedia.org/wiki/National_research_and_education_network) organization primarily funded by Goverment of Alberta and other Canadian government agencies. Cybera provides IT services for University, K-12, and startup entrepreneurs.

I live in Calgary, Alberta, Canada, which is underrated as an amazing city for the outdoors enthusiast. We are in close proximity to the beautiful Canadian Rockies, and any mountain sport you can think of is available here.

## Open Source Projects

When I was learning Rust, I decided to work on a project to make the learning process more tangible and focused. The goal of my project was to write to an LED matrix on a Raspberry Pi in Rust. For the final working project, you can see my GitHub repo [writeLED-rs](https://github.com/anna-liao/writeLED-rs). I also presented on this project at the inaugural PyCascades 2018: [RaspberryPy to RustyPi](https://www.slideshare.net/secret/lUQ7YxnKo6C8Od).

I was an [Outreachy](https://www.outreachy.org/) intern with The Wikimedia Foundation from Nov 2016 to March 2017. I worked on a parser for the Python open source project Pyslet and you can read more at my [project wiki](https://github.com/anna-liao/pyslet/wiki).

## Lawrence Berkeley Lab

I was an engineer supporting research to inform energy policy. I worked on projects in the areas of 1) energy efficiency in residential and small commercial buildings and 2) smart grid and distribution grid.

Some cool projects I worked on during this time:

* **[Monitoring residential hot water consumption.](https://aceee.org/files/proceedings/2014/data/papers/1-187.pdf)** The purpose of this project was to examine energy and water waste of residential hot water distribution systems. We made our own flowmeters to monitor water flow at 1 second resolution. We deployed a wireless sensor network in multiple homes to monitor water flow at all water end uses and energy consumption of the water heater. This was streamed to our server at LBL such that we could view real-time consumption. An example of what we could determine with this data is how long a person left the hot water tap on before a shower (and that corresponds to water and energy waste). 

* **[Demonstrating a low-cost device to enable demand response (DR) for 1 kW dinky loads.](http://aceee.org/files/proceedings/2014/data/papers/11-183.pdf)** Traditionally, a system to enable DR in a 1 MW aluminum smelter costs $50k. This is because if the electric utility is counting on shedding 1 MW load, the DR device must reliably shut off that load. Most of the cost of that system is to ensure reliability. The goal of our project is to demonstrate a low cost (approx. $100) device to enable DR for all the 1 kW "dinky loads" such as the community theater or small office building. Even if we can get 90% reliability, then we can shed 900 kW in 1000 dinky loads. For this project, we deployed embedded PCs in remote buildings that can receive DR signals to shut off load remotely by controlling the thermostat.

* **[Micro-synchrophasors for insight at the distribution grid level](https://gig.lbl.gov/sites/all/files/lbnl-1005925.pdf)** The U.S. Dept. of Energy is looking to [modernize the power grid](https://www.energy.gov/grid-modernization-initiative). The power grid we have now is not designed for all the solar, electic vehicles, and other distributed energy resources feeding energy into the grid. The old grid model mostly only has sensors and visibility at the transmission level. The objective of a micro-synchrophasor is to add sensors at the distribution level. Currently, when there is a power issue, someone drives out to the location to manually assess the situation and (hopefully) fix it. For this project, we demonstrated a device that is installed at the distribution substation that can identify the source of voltage sags and other power issues in the distribution system. This would make it faster to identify problems. Some fun incidents that we observed while I was on the project is identifying causes for why there was a voltage sag. In one case, it was a hawk carrying a mouse that was zapped by the power line... and yes, they found the fried specimen.

![pycon2017](/images/blog/about/pycon2017.jpg)
_Presenting a poster on my LBL work at PyCon 2017_

## NASA Jet Propulsion Lab

I was a microdevices engineer working on sensor microfabrication. I _really_ liked the applications for my work, which included high temperature and radiation hard sensors and electronics for Venus. I attained many valuable skills at JPL including builing sensor prototypes end-to-end, optical and electrical characterization and data analysis.
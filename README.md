## Foot Traffic Modeling of the 2nd Floor at Namsan Library

### Table of Contents
1. [About Namsan Library (2nd Library)](#about-namsan-library-2nd-library)
2. [Figure 1: Interactive Virtual Tour in Figma](#figure-1-interactive-virtual-tour-in-figma)
3. [Figure 2: Site Map of Namsan Library’s 2nd Floor](#figure-2-site-map-of-namsan-librarys-2nd-floor)
4. [Data Collection Method Procedure](#data-collection-method-procedure)
5. [Acknowledging Limitations](#acknowledging-limitations)
6. [Foot Traffic – Quantitative Analysis](#foot-traffic-quantitative-analysis)
7. [Putting Results into Context](#putting-results-into-context)
8. [Appendix](#appendix)

---

### About Namsan Library (2nd Library)
Our selection of the Seoul Namsan Library for our traffic model is influenced by South Korea's academic culture. The educational system in South Korea is known for its rigorousness, with a high value placed on academic achievement and learning. An outcome of this system is the Suneung, the highly competitive national university entrance exam. The intense preparation for Suneung fosters an environment where libraries become essential to students.

In this context, the Seoul Namsan Library, located near the iconic Seoul Tower, a popular tourist and cultural site, stands as an ideal representation of this academic phenomenon. The library's proximity to a significant landmark suggests a potentially high and diverse foot traffic, making it a fitting model for our assignment. Additionally, the library's diverse functional areas – including a book cafe, outdoor library, numerous seating areas, a printing zone, and a PC area – provide a rich framework for analyzing varied foot traffic patterns.

Though an official floor plan is absent, we developed an Interactive Virtual Tour using Figma. This allowed us to virtually present the library's layout and key areas for improved accuracy and understanding of our analysis.

---

### Figure 1: Interactive Virtual Tour in Figma
Note: This interactive tour provides a virtual walkthrough of Seoul Namsan Library, highlighting key areas and pathways, and offering an immersive view of the library's layout. [Take the tour here](#).

---

### Figure 2: Site Map of Namsan Library’s 2nd Floor
Note: There are areas that cannot be physically accessed without going through another node. These are represented by the lack of an arrow. In the matrix, these are represented with a value of zero.

---

### Data Collection Method Procedure
Our data collection at Seoul Namsan Library was conducted on November 14, 2023. It was a Tuesday afternoon, towards the end of the Fall season. We worked on other assignments in the library from 2.45 p.m. to 5 p.m. During this period, we systematically collected data at three key intervals: 2.45 p.m., 4 p.m., and 5 p.m.

Our method involved manually counting the number of people present in each of the library's designated areas (nodes):
- Entrance
- Book Cafe
- Outdoor Library
- Seating Area beside the library
- Printing Area
- PC Zone

To ensure accuracy and consistency, we used alarms to remind us to conduct the counts at the specified intervals.

---

### Acknowledging Limitations
We recognize that our assignment has certain limitations. The data was collected on a single weekday and during a specific season, which may not fully represent the library's foot traffic at different times or under varying conditions. We suggest that future models could expand the scope of data collection to include different days of the week, as well as various seasons, to capture a more comprehensive picture of the library's usage patterns.

---

### Foot Traffic – Quantitative Analysis
In our analysis of the Seoul Namsan Library's foot traffic, we used a matrix M, representing the normalized traffic flow between different areas of the library. By raising this matrix to higher powers and multiplying it by various initial distributions, we observed how the system evolves over time towards a steady state. This steady state closely aligns with the eigenvector corresponding to the largest eigenvalue of M.

The library's foot traffic reaches a steady state where about 11.61% of visitors are at the entrance, 16.52% in the Book Cafe, 13.84% outdoors, 34.82% in the seating area, 5.36% in the Printing Area, and 17.86% in the PC Zone.

Visitors start predominantly (1) at the entrance, (2) are concentrated in reading areas, or (3) are using library services. As we apply the matrix M repeatedly (simulating the passage of time), the influence of these initial conditions diminishes. Eventually, the system converges to a distribution that is almost identical to the dominant eigenvector of M. This convergence indicates that, regardless of where visitors start, the foot traffic distribution across the library stabilizes into a predictable pattern over time. It is a direct reflection of the dominant eigenvector with the eigenvalue of 1, which represents the steady state of the system.

This model, while insightful, operates under the assumption that the library is a closed system with minimal entries and exits during the observed period. This assumption might not hold in real-world scenarios, where new visitors continuously enter, and others leave. To accommodate this, we could introduce additional factors into our model. For instance, we could incorporate a constant rate of entry and exit for each area, adjusting our matrix accordingly. This would allow the model to account for the dynamic nature of foot traffic, providing a more realistic representation of how the system evolves.

---

### Putting Results into Context
Understanding that, in the long run, the highest concentration of visitors (34.82%) will be in the seating area, while the lowest (5.36%) will be in the Printing Area, can guide resource allocation and space management decisions. These results underscore the importance of considering long-term traffic patterns in library management and layout planning. By anticipating where visitors are most likely to congregate, library administrators can optimize space and resources to enhance the visitor experience.

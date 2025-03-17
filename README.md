# Website
Portfolio
install.packages("shiny")
library(shiny)

ui <- fluidPage(
  titlePanel("Angela Orokoh | Portfolio"),
  
  navbarPage("", 
             tabPanel("Home", 
                      fluidRow(
                        column(12, h2("About Me")),
                        column(12, p("My name is Angela Jones-Orokoh. I am a rising 3rd year PhD student at the University of Chicago Crown School of Social Work, Policy, and Practice. I study racial, economic, and spatial inequality, particularly in the context of housing, neighborhood change, and public policy. My research, which takes a transdisciplinary approach and utilizes quantitative, computational, and historic-comparative methods, is aimed at investigating the multifactorial conditions of housing. In my current research, I focus on African American applied heuristics of the ‘right to the city’ within the United States and the spatial expressions and productions of self-determination within the urban context."))
                      )
             ),
             
             tabPanel("Current Focus", 
                      fluidRow(
                        column(12, h2("Labor Shifts, Housing Shocks: Examining Employment Precarity as a Risk Factor in Housing Instability and Household Related Hardships")),
                        column(12, h4("Abstract")),
                        column(12, p("Extensive research has demonstrated a robust association between income and housing-related hardship. However, less is known about the extent to which precarious employment serves as a predictor of housing instability and material deprivation. This study examines how shifts in the labor market—particularly the rise of nonstandard, contingent, and unstable employment—contribute to housing instability and related hardships. ")),
                        column(12, p("Drawing on data from 3,171 respondents in wave five of the Future of Families and Child Wellbeing Study, this analysis operationalizes precarious employment as a multidimensional construct, incorporating five subjective indicators (nonstandard schedules, working ≤35 hours per week, non-traditional hours, irregular shifts, and multiple jobs). Structural equation modeling (SEM) is employed to validate the composite measure, which is subsequently used in logistic regression models to assess its relationship with four distinct manifestations of housing instability: unaffordability, doubling up, eviction, and homelessness.")),
                        column(12, p("Findings indicate that, after adjusting for relevant covariates, individuals in precarious employment face a heightened likelihood of missing rent or mortgage payments and residing in shared living arrangements due to financial constraints. However, no statistically significant association emerges between precarious employment and the risk of eviction or homelessness. Beyond these housing instability indicators, precarious employment is also linked to increased exposure to material hardships, including borrowing money to meet basic expenses, utility payment delinquency, food insecurity, and telephone service disconnection.")),
                        column(12, p("Notably, the significant associations persist even after controlling for household income suggesting that employment precarity exacerbates housing vulnerabilities beyond earnings alone. These findings underscore the urgent need to address labor market conditions to mitigate housing instability, reinforcing the need to assess labor and housing related processes."))
                      )
             ),
             
             tabPanel("CV", 
                      fluidRow(
                        column(12, h2("Curriculum Vitae")),
                        column(12, p("Download my CV here: ", a("Angela Orokoh - CV", href="https://drive.google.com/file/d/18r683U84v0c3YUG9kG4-Kvu28yHowaZS/view?usp=drive_link", target="_blank")))
                      )
             ),
             
             tabPanel("Contact", 
                      fluidRow(
                        column(12, h2("Contact Me")),
                        column(12, p("Email: aorokoh@uchicago.edu")),
                        column(12, p("Phone: 414-627-6223"))
                      )
             )
  ) 
) 

server <- function(input, output) {}

shinyApp(ui = ui, server = server)

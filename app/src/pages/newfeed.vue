<template>
    <div class="activities-app">
        
        <company v-bind:company_data="company_data"/>
        
        <contacts/>
    </div>
</template>

<script>
export default {
    name: 'newfeed',
    data() {
        return {
            company_data: {
                days: [
                    {
                        day_name: 'Monday, 9th',
                        day_number: '9',
                        border_color: '#D1E71C',
                        sessions: [
                            {
                                company: "BCG",
                                company_link: "https://www.youtube.com/embed/eYbolHBNC5c",
                                description: "Boston Consulting Group partners with leaders in business and society to tackle their most important challenges and capture their greatest opportunities. BCG was the pioneer in business strategy when it was founded in 1963. ",
                            },
                            {
                                company: "Outsystems",
                                company_link: "https://www.youtube.com/embed/0gx3hMMDOZI",
                                description: "OutSystems is a low-code platform to visually develop your application, integrate with existing systems and add your own code when needed.",
                                show: true
                            },
                        ]
                    },
                    {
                        day_name: 'Tuesday, 10th',
                        day_number: '10',
                        border_color: '#D1E71C',
                        sessions: [
                            {
                                company: "Deloitte",
                                company_link: "https://www.youtube.com/embed/LN_TjdcAEEg",
                                description: "We provide audit & assurance, consulting, financial advisory, risk advisory and tax through the following separate and legally distinct subsidiaries and affiliates of Deloitte",
                                show: true
                            },
                            {
                                company: "Critical TechWorks",
                                company_link: "https://www.youtube.com/embed/wCfTVQBeiPE",
                                description: "Critical TechWorks is a joint venture to lead the future of motion. Established in 2018, Critical TechWorks is a company formed as a result of a partnership between BMW Group and Critical Software. Critical TechWorks is exclusively put together to support BMW in building software for its future driving machines.",
                                show: true
                            },
                        ]
                    },
                    {
                        day_name: 'Wednesday, 11th',
                        day_number: '11',
                        border_color: '#D1E71C',
                        sessions: [
                            {
                                company: "KPMG",
                                company_link: "https://www.youtube.com/embed/vUt1aaLxLuY",
                                show: true
                            },
                            {
                                company: "Accenture",
                                company_link: "https://www.youtube.com/embed/SAj32bRdwws",
                                show: true
                            },
                        ]
                    },
                    {
                        day_name: 'Thursday, 12th',
                        day_number: '12',
                        border_color: '#D1E71C',
                        sessions: [
                            {
                                company: "Vodafone",
                                company_link: "https://www.youtube.com/embed/suH5nmmHhuE",
                                show: true
                            },
                            {
                                company: "Microsoft",
                                company_link: "https://www.youtube.com/embed/T44F3N9p9rY",
                                show: true
                            },
                        ]
                    },
                ]
            },
        }
    }           
}
</script>

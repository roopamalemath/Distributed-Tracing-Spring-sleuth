# Distributed-Tracing-Spring-sleuth

Spring-cloud-sleuth - assign a unique id to the request so that i can trace the request across the multiple components.

steps for implementation of spring - cloud - sleuth

1. add a dependency

<dependency>
			<groupId>org.springframework.cloud</groupId>
			<artifactId>spring-cloud-starter-sleuth</artifactId>
		</dependency>
    
 2. trace all the request we want to create something called Sampler
 
 @Bean
	public Sampler defaultSampler() {
		return Sampler.ALWAYS_SAMPLE;
	}
  
